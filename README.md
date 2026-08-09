# homelab
My Homelab setup documented and organized to the best of my abilities

------------------------------------
Proxmox Env

PVEmini
i3-1220P, 16gb ram, 500gb ssd
runs media server and most higher compute services

PVElong
CPU E3-1230 V2, 32gb of ram, lots of drives
12x HDD bays currently has 7 occupied for approx 50tb raw in a mergefs array

------------------------------------

Kub Cluster
k3s powered cluster running debian as the base OS

3 control plane nodes 
4vCPU, 4GB ram, 16gb drive
virtual machine on my proxmox env 2 PVElong 1 on the PVEmini for better availability

3 worker nodes
HP EliteDesk 800 G3 Mini, i5-6500t, 8gb RAM, 128gb boot SSD, 500GB ssd for longhorn
phsyical nodes running all my worker pods with distrubed storage and high availabity for my internal and external services

------------------------------------

The start of the YAML was written with help of ai but as my skills grew I began to write it myself based on templates from online and AI

the EXT Folder is all of my externally accessible items that are also behind a bunkerweb instance for higher security

The apps folder are all of my manifests I feel comfortable posting publically

template-full-storage.yaml is what I use as a starting point for new pod deployments


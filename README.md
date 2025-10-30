# homelab
My Homelab setup documented and organized to the best of my abilities


Proxmox Env

Beelink mini pc
i3-1200p, 16gb ram, 500gb ssd
runs media server and most higher compute services

1u storage server
12x HDD bays currently has 7 occupied for approx 50tb raw in a mergefs array


Kub Cluster
3 control plane node - virtual machine on my proxmox env 2 on one host 1 on the other
3 worker nodes -  HP G3 mini PCs running talos linux

The start of the YAML was written with help of ai but as my skills grew I began to write it myself based on templates from online and AI


the EXT Folder is all of my externally accessible items that are also behind a bunkerweb instance for higher security, everything else is purly internal. 
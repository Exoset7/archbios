
# Fucking French Archlinux Custom Install - BIOS - MBR

Before continuing : read this example for prepare the disk  (dos mode)
The following partitions are required with dos mode  ( you can use cfdisk tools for that)

      /dev/sdaXXXXXX1     500G       type :  Linux FileSystem
  
Format the partitions

     mkfs.ext4 /dev/sdaXXXXXX1
  
Mount the root partition file systems

    mount /dev/sdaXXXXXX1 /mnt

    sudo pacman -Sy
    sudo pacman -S git
    git clone https://github.com/Exoset7/archbios.git
    cd archbios
    chmod +x archbios.sh
    ./archbios.sh

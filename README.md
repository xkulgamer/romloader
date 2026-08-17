
## romloader 
- romloader is a qemu wrapper designed for running android roms.
- romloader is in beta state.
- current version: v0.1 beta
- you can do anything to this program, please refer to the license for more details.
## dependencies
```
qemu-system-aarch64
abootimg
```
on debian/apt-based systems, you can install them with the following command:
```
sudo apt install qemu-system-aarch64 abootimg
```
if you haven't yet, please update your repository list.

in arch-based systems you can install the dependencies using the following commands: 
```
sudo pacman -S qemu-full
sudo yay -s abootimg
```
in fedora-based systems you can install the dependencies using the following command:
```
sudo dnf install qemu-system-aarch64 abootimg
```
## usage
get a android rom zip and extract it, then, do the following commands in the directory where you cloned romloader:
```
./unpack your-boot.img
./flash system your-system.img
./flash userdata sizeofuserdata
./qemu addkernel your-kernel
./qemu config ram ramsize
./qemu start
./qemu serial
```
now you know how to use romloader and set it up! 



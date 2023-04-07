# win_unpacker
Android System Unpacker Script by Yoti

Extract system folder from system.new.dat.br or system.new.dat
Copy all the files (sda2img) in this branch to where system.new.dat.br or system.new.dat are extracted. Then follow the guide at each step. If you wanna extract system.new.dat then start from Extract system.new.dat unless start from beginning.

Supports:

system.new.dat.br
system.new.dat
all android version ROM :-)
Extract system.new.dat.br
sudo apt install brotli

brotli --decompress system.new.dat.br -o system.new.dat

Extract system.new.dat
./sdat2img.py system.transfer.list system.new.dat system.img
Extract system.img
mkdir output

sudo mount -t ext4 -o loop system.img output/

Gaining Permission Of Extracted system folder
sudo chown -R USERNAME:USERNAME ~/path/of/mounted/image
{Eg:} sudo chown -R hardik:hardik ~/Documents/ROM/final/Extracted/output

-_- Booyah! You got the system folder.Now Copy all the files from output folder to any other place.

Deleting Output Folder
Run these commands where the output folder exists.

sudo umount output

sudo rm -rf output


Done! Thank Me Later
Credits
StackOverFlow

XDA

G O D

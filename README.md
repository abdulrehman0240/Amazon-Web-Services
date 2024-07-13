# Amazon-Web-Services
--Adding New Volume--
$lsblk | Show harddisk and system partition
Goto AWS Console-> EC2 Instance -> Volumes -> Create Volume ->
-> Select volume type -> gp2 -> same availability zone as EC2 ->
-> <10>GB -> Create volume

Select volume -> Attach volume -> 
$lsblk 
$file -s /dev/<xvdf> | If show data it is raw disk
$sudo mkfs -t ext4 /dev/<xvdf> | Format and save filesystem
$sudo lsblk | check
$sudo mkdir /<fileserver> 
$sudo mount /dev/xvd<f> /fileserver/
$sudo lsblk
$cd /fileserver
$sudo nano abc | Type something and Ctrl+O Ctrl+X
$sudo cat abc


### Enable auto-login
- Settings > Users > Unlock
- Automatic Login ON
### Disable screen lock
- Settings > Privacy > Screen Lock
- Automatic Screen Lock OFF
### Install guest additions
- (VirtualBox) Devices > Insert Guest Additions CD Image...
- ```bash
   su
   apt install linux-headers-$(uname -r)
   apt install gcc make perl
   mount -o remount,exec /media/cdrom0
   cd /mnt/cdrom0
   bash -x ./VBoxLinuxAdditions.run
   ```
### Set up sudo
   ```bash
   su
   apt install sudo
   usermod -aG username
   ```

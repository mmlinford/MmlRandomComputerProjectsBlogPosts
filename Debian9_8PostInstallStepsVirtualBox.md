
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
   apt install linux-headers-$(uname -r) gcc make perl
   mkdir GuestAdditions
   cp -rf /mnt/cdrom/* GuestAdditions/
   cd GuestAdditions
   ./VBoxLinuxAdditions.run
   ```
### Set up sudo
   ```bash
   su
   apt install sudo
   usermod -aG username
   ```

# macbook-android-mobile-backup
Steps to backup your android to your Mac book

Android configuration
- Install SSHelper 
- Start sftp server
- SD Maid (for the undeletable files)

Macbook configuration
- Install CyberDuck
- Open connection on remote mobile sftp server

Transfer process
- Use Cyberduck's easy ui
- From the terminal: rsync --remove-source-files -av -zz --progress  -e 'ssh -p 2222' admin@192.168.1.44:/storage .

Rsync update (if v < v.3.1.3 to have the compression) <br>
https://apple.stackexchange.com/questions/344324/update-rsync-in-high-sierra <br>
https://apple.stackexchange.com/questions/359821/whats-the-best-way-to-update-homebrew-when-upgrading-macos

Backup paths
/storage/emulated/0/Whatsapp Videos/
/storage/emulated/0/Whatsapp Images/

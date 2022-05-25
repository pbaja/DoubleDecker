# 📦 Enabling SSH to transfer files

## Enabling SSH
The default deck user is shipped with no password. This is a secure setting that prevents access via ssh, and can't be used to run commands via sudo.
We need to change that.

1. Head over to Applications -> System -> Konsole
2. Enter `passwd` command and hit Enter
3. Enter your new password (Typed characters do not apper on the screen) and hit Enter
4. Retype the password and hit Enter
5. Done! Your account now should have a password

Now need to enable the ssh with this simple command, this would make the ssh server start at boot:
```
sudo systemctl enable sshd
```
After that, run this command to start the server immediately:
```
sudo systemctl start sshd
```
Now, on your computer, you should be able to access the Steam Deck terminal with this command:
```
ssh deck@steamdeck.local
```
Note: If your router is not catching up with the domain name, you must type the SteamDeck's IP address manually instead of the `steamdeck.local`. You can easily check the IP address by typing `ip addr`

## Transferring files
If you have a linux machine this should be a pretty straightforward for you - just mount the remote directory.
On Windows you can use this amazing tool called [WinSCP](https://winscp.net/eng/download.php).
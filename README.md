# ssh-mfa-pam-google
SSH 2FA AUTH With Google PAM

# Install Google Authenticator PAM
```
sudo apt-get install libpam-google-authenticator -y
```


root@anish-ubuntu:/home/adminuser# google-authenticator 

Do you want authentication tokens to be time-based (y/n) y
https://www.google.com/chart?chs=200x200&chld=M|0&cht=qr&chl=otpauth://totp/root@anish-ubuntu%3Fsecret%3DUXCRH65GUL6VM7OJ

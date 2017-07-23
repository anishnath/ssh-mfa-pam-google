# ssh-mfa-pam-google
SSH 2FA AUTH With Google PAM

# Install Google Authenticator PAM
```
sudo apt-get install libpam-google-authenticator -y
```


root@anish-ubuntu:/home/adminuser# google-authenticator 

Do you want authentication tokens to be time-based (y/n) y
`
https://www.google.com/chart?chs=200x200&chld=M|0&cht=qr&chl=otpauth://totp/root@anish-ubuntu%3Fsecret%3DUXCRH65GUL6VM7OJ
`
![QRCODE](https://github.com/anishnath/ssh-mfa-pam-google/blob/master/QR.png)

```
Your new secret key is: UXCRH65GUL6VM7OJ
Your verification code is 624801
Your emergency scratch codes are:

  53655489
  52378031
  85704939
  31102683
  64239395

Do you want me to update your "/root/.google_authenticator" file (y/n) y

Do you want to disallow multiple uses of the same authentication
token? This restricts you to one login about every 30s, but it increases
your chances to notice or even prevent man-in-the-middle attacks (y/n) y

By default, tokens are good for 30 seconds and in order to compensate for
possible time-skew between the client and the server, we allow an extra
token before and after the current time. If you experience problems with poor
time synchronization, you can increase the window from its default
size of 1:30min to about 4min. Do you want to do so (y/n) y

If the computer that you are logging into isn't hardened against brute-force
login attempts, you can enable rate-limiting for the authentication module.
By default, this limits attackers to no more than 3 login attempts every 30s.
Do you want to enable rate-limiting (y/n) y

```

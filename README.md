Scripts for cracking / bruteforcing.

## Password generator
Generate a list of possible password for a company name. The name of company should be in lowercase (script will generate the iterations in uppercase). Use like this:
```sh
user@hostname:~/bin/passtool$ ./generator name
```
### Example
```sh
user@hostname:~/bin/passtool$ ./generator google
google1
google2015
google2014
...
```

## Feed wordlist
Append new passwords from a file to your custom big wordlist. Script also remove duplicates for both files, so you don't have to clean none of the files.
```sh
user@hostname:~/bin/passtool$ ./feed_wordlist rockyou_custom.txt passwords.txt
```
### Example
```sh
user@hostname:~/bin/passtool$ ./feed_wordlist rockyou_custom.txt google_passwords.txt
[*] uniq new password file...
[*] Feeding original wordlist with password file
[*] uniq new wordlist ...
[!] /home/user/bin/passtool/rockyou_custom.txt.18Aug2018 file has been created.
```

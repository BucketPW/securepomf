# securepomf
Encrypted uploads to pomf.se.

If ran on a file, it will generate a strong but URL-friendly password, encrypt the file, upload it, and return the URL with the password appended.

If ran on one such password-containing URL, it will download that file and decrypt it, saving to the current directory.


```
$ ./securepomf diceware8k.txt

Encrypting diceware8k.txt...
Uploading encrypted file...
Upload attempt #0... Uploaded!
File has been encrypted and uploaded to: http://a.pomf.se/gslbrg.txt#j6Vp6_BvPtE5xb7dz9ecBj2C-tzc9WyO


$ ./securepomf http://a.pomf.se/gslbrg.txt#j6Vp6_BvPtE5xb7dz9ecBj2C-tzc9WyO

Downloading and decrypting gslbrg.txt...
File saved to: gslbrg.txt
```

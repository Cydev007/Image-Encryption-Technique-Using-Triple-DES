# Image-Encryption-Technique-Using-Triple-DES
### Introduction 
Triple DES is a encryption technique which uses three instance of DES on same plain text. Triple Data Encryption Algorithm (TDEA or Triple DEA), is a symmetric-key block cipher, which applies the DES cipher algorithm three times to each data block.


### Algorithm


Encrypt the plaintext blocks using single DES with key K1.
Now decrypt the output of step 1 using single DES with key K2.
Finally, encrypt the output of step 2 using single DES with key K3.
The output of step 3 is the ciphertext.
Decryption of a ciphertext is a reverse process.

![image](https://user-images.githubusercontent.com/108612723/180634707-dcfc4005-b797-47da-bdc8-fce1e2863d6e.png)

### Functionality
**Can decrypt and encrypt Images using DES alogrithm**

Advantages The image can only be viewed by the receiver as the image is encrypted using Triple DES and the key is only known to the sender and receiver. Since the image is encrypted using Triple DES, it is more secure than DES. Since the key is entered by the sender and receiver and is not stored in the database, it makes the encryption and decryption more secure.


Password hashing - PBKDF2 used(I will welcome advanced modes)
Salting done
Hashing and salting password performed multiple times (>10,000)
Digital signature in form of SHA256 used
CBC (Cipher block chaining used) - triple DES
Initialization vector for CBC is derived from the password hash itself.

Make sure to uninstall all versions of crypto and pycrypto first, then install pycryptodome:

	pip3 uninstall crypto 
	pip3 uninstall pycrypto 
	pip3 install pycryptodome

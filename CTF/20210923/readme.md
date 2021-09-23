# 3_1_2_python現代密碼實測_pycrypto
- [Pycrypto](https://github.com/JimLi999/CS2021/tree/main/CTF/20210923#Pycrpto)
- [AES對稱式加解密](https://github.com/JimLi999/CS2021/tree/main/CTF/20210923#aes%E5%B0%8D%E7%A8%B1%E5%BC%8F%E5%8A%A0%E8%A7%A3%E5%AF%86)

## Pycrypto
- [Install pycrypto](https://github.com/JimLi999/CS2021/tree/main/CTF/20210923#install-pycrpto)
- [Module number](https://github.com/JimLi999/CS2021/tree/main/CTF/20210923#module-number)
- [Get Greatest Common Divisor by pycrypto](https://github.com/JimLi999/CS2021/tree/main/CTF/20210923#get-greatest-common-divisor-via-pycrypto)

### Install pycrypto
```python
pip install pycrypto
```
![result](./pycrypto_install.PNG)

### Module number
- [Module number](https://pythonhosted.org/pycrypto/Crypto.Util.number-module.html)

### Get Greatest Common Divisor via pycrypto
透過 pycrypoto 函數庫取得最大公約(因)數
```python
from Crypto.Util.number import GCD

GCD(12,18)
```
![result](./getGCD.PNG)

## AES對稱式加解密
- [AES Encrypt](https://github.com/JimLi999/CS2021/tree/main/CTF/20210923#aes-encrypt)
- [AES Decrypt](https://github.com/JimLi999/CS2021/tree/main/CTF/20210923#aes-decrypt)

### AES Encrypt
```python

from Crypto.Cipher import AES

obj = AES.new('This is a key123', AES.MODE_CBC, 'This is an IV456')

message = "flag(HappyCrypt)"

ciphertext = obj.encrypt(message)
ciphertext
```
![result](./AES_encrypt.PNG)
### AES Decrypt
```python
obj2 = AES.new('This is a key123', AES.MODE_CBC, 'This is an IV456')

obj2.decrypt(ciphertext)
```
![result](./AES_decrypt.PNG)



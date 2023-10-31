# Play Nice

## Problem
Not all ancient ciphers were so bad... The flag is not in standard format. nc mercury.picoctf.net 19354 playfair.py


## Solution
1. Open Terminal and connect to `nc mercury.picoctf.net 19354` 
2. You will get the following output: 


```
Here is the alphabet: meiktp6yh4wxruavj9no13fb8d027c5glzsq
Here is the encrypted message: y7bcvefqecwfste224508y1ufb21ld
What is the plaintext message?
```
3. After that go to [dCode](https://www.dcode.fr/en) and put the appropriate parameters for PlayFair Cipher.
4. You should get `7V8441MFRERHDR8RH20F2FYA20NOAQ` as the Result.
5. Convert it to lowercase and input this as the plaintext message and you get the flag.


## Flag

`dbc8bf9bae7152d35d3c200c46a0fa30`
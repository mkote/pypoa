# padding-oracle-decrypter
Tool for decrypting CBC encrypted ciphertexts using the padding oracle attack

```
import decrypt
from decrypt import OracleAttack

data = b"secret"
key = b"Sixteen byte key" 
iv = b"/kQ\x0bDZ\xc6F\xb2\xc4\x9c\xca\x8c\'!]"
cipherText = b'VS&\xcb\xa7\xa5<\x14d\x00j\xe6\xb5\xba\xad\x08'
ct = iv+cipherText
attack = OracleAttack()
decrypted = attack.execute(iv+cipherText)
 ```

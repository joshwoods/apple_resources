

- Device Management
- PasswordHash
-  PasswordHash.SALTED-SHA512-PBKDF2 

Object

# PasswordHash.SALTED-SHA512-PBKDF2

A dictionary that contains the elements you use to create the password hash.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object PasswordHash.SALTED-SHA512-PBKDF2
```

## Properties

`entropy`

`data`

 (Required) 

The derived key from the password hash; for example, from `CCKeyDerivationPBKDF()`.

`iterations`

`integer`

 (Required) 

The number of iterations; for example, from `CCCalibratePBKDF()` using a minimum hash time of 100 milliseconds, or if unknown, a number in the range of 20,000 to 40,000 iterations.

`salt`

`data`

 (Required) 

The 32-byte randomized data; for example, from `CCRandomCopyBytes()`.




- Security
-  kSecKeyEffectiveKeySize 

Global Variable

# kSecKeyEffectiveKeySize

Type uint32; value is the effective number of bits in this key. For example, a DES key has a key size in bits (`kSecKeyKeySizeInBits`) of 64 but a value for `kSecKeyEffectiveKeySize` of 56.

macOS 10.0+

``` source
var kSecKeyEffectiveKeySize: Int32 { get }
```


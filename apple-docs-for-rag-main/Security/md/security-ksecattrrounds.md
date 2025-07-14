

- Security
-  kSecAttrRounds 

Global Variable

# kSecAttrRounds

A key whose value indicates the number of rounds to run the pseudorandom function.

macOS 10.7+

``` source
let kSecAttrRounds: CFString
```

## Discussion

The corresponding value is of type CFNumber and indicates the number of rounds to run the pseudorandom function specified by kSecAttrPRF for a cryptographic key.


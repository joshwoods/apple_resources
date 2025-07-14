

- Security
-  kSecCodeInfoDigestAlgorithm 

Global Variable

# kSecCodeInfoDigestAlgorithm

A key whose value is a number indicating the cryptographic hash function.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoDigestAlgorithm: CFString
```

## Discussion

The value is a CFNumber indicating the kind of cryptographic hash function used within the signature to seal its pieces together. See SecCSDigestAlgorithm for possible value.


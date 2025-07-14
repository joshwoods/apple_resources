

- Security
-  kSecCodeInfoCdHashes 

Global Variable

# kSecCodeInfoCdHashes

A key whose value is an array containing the unique binary identifier for every digest algorithm supported in the signature.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoCdHashes: CFString
```

## Discussion

The corresponding CFArray contains the values of the kSecCodeInfoUnique binary identifier for every digest algorithm supported in the signature in the same order as in the kSecCodeInfoDigestAlgorithms array. The kSecCodeInfoUnique value contained in this array corresponds to the kSecCodeInfoDigestAlgorithm value.


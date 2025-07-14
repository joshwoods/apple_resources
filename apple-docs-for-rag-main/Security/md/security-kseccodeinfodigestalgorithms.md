

- Security
-  kSecCodeInfoDigestAlgorithms 

Global Variable

# kSecCodeInfoDigestAlgorithms

A key whose value is a list of the kinds of cryptographic hash functions available within the signature.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoDigestAlgorithms: CFString
```

## Discussion

The value is a CFArray of CFNumber objects indicating the kinds of cryptographic hash functions available within the signature. The ordering of the items in the array has no significance in terms of priority, but determines the order in which the hashes appear in kSecCodeInfoCdHashes.




- Security
-  kSecPaddingOAEPKey Deprecated

Global Variable

# kSecPaddingOAEPKey

PKCS7 padding will be used when encrypting or decrypting.

macOS 10.8–13.0Deprecated

``` source
let kSecPaddingOAEPKey: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

When using this padding type, consider also setting the kSecOAEPMessageLengthAttributeName, kSecOAEPEncodingParametersAttributeName, and kSecOAEPMGF1DigestAlgorithmAttributeName attributes.


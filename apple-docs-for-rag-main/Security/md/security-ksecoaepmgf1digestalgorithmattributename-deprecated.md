

- Security
-  kSecOAEPMGF1DigestAlgorithmAttributeName Deprecated

Global Variable

# kSecOAEPMGF1DigestAlgorithmAttributeName

The OAEP MGF1 digest algorithm.

macOS 10.7–13.0Deprecated

``` source
let kSecOAEPMGF1DigestAlgorithmAttributeName: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Set this value to one of the digest algorithms listed in Digest Types when the kSecPaddingKey attribute is set to kSecPaddingOAEPKey. If you don’t set this attribute, kSecDigestSHA1 is used by default.

This attribute is ignored when padding is not set to OAEP.


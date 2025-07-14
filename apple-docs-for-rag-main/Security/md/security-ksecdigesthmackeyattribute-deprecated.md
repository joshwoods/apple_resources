

- Security
-  kSecDigestHMACKeyAttribute Deprecated

Global Variable

# kSecDigestHMACKeyAttribute

The key for HMAC operation.

macOS 10.7–13.0Deprecated

``` source
let kSecDigestHMACKeyAttribute: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

The value is a CFData object that specifies the key when kSecDigestTypeAttribute attribute is set to one of the HMAC options listed in Digest Types. If this value is not set, the transform will assume a zero length key.


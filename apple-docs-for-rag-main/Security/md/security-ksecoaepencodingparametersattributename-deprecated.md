

- Security
-  kSecOAEPEncodingParametersAttributeName Deprecated

Global Variable

# kSecOAEPEncodingParametersAttributeName

The OAEP encoding parameters.

macOS 10.7–13.0Deprecated

``` source
let kSecOAEPEncodingParametersAttributeName: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Set this value to a CFData object when the kSecPaddingKey attribute is set to kSecPaddingOAEPKey. If you don’t set this attribute, a zero length data object is used by default.

This attribute is ignored when padding is not set to OAEP.




- Security
-  kSecOAEPMessageLengthAttributeName Deprecated

Global Variable

# kSecOAEPMessageLengthAttributeName

The OAEP message length.

macOS 10.7–13.0Deprecated

``` source
let kSecOAEPMessageLengthAttributeName: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Optionally set the value to a CFNumber indicating a specific message size when the kSecPaddingKey attribute is set to kSecPaddingOAEPKey. If you don’t set this attribute, the minimum padding is used by default.

This attribute is ignored when padding is not set to OAEP.


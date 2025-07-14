

- Security
-  kSecTransformActionAttributeValidation Deprecated

Global Variable

# kSecTransformActionAttributeValidation

An action that triggers to perform validation of an attribute.

macOS 10.7–13.0Deprecated

``` source
let kSecTransformActionAttributeValidation: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Allows a block to be called to validate the new value for an attribute. The default is no validation and any CFTypeRef can be used as the new value. The block should return NULL if the value is ok to set on the attribute or a CFErrorRef otherwise.


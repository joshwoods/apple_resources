

- Security
-  kSecTransformActionProcessData Deprecated

Global Variable

# kSecTransformActionProcessData

An action that triggers to process the data of an attribute.

macOS 10.7–13.0Deprecated

``` source
let kSecTransformActionProcessData: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Overrides the standard data processing for an attribute. This is almost exclusively used for processing the input attribute as the return value of their block sets the output attribute. This is used with the SecTransformOverrideAttributeAction block.


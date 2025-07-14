

- Security
-  kSecTransformActionAttributeNotification Deprecated

Global Variable

# kSecTransformActionAttributeNotification

An action that triggers when an attribute is set.

macOS 10.7–13.0Deprecated

``` source
let kSecTransformActionAttributeNotification: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Allows a block to be called when an attribute is set. This allows for caching the value as a block variable in the instance block or transmogrifying the data to be set. This action is where a custom transform would be able to do processing outside of processing input to output as process data does. One the data has been processed the action block can call SecTransformCustomSetAttribute to update and other attribute.


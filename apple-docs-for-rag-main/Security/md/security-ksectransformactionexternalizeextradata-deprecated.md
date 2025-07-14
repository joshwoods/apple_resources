

- Security
-  kSecTransformActionExternalizeExtraData Deprecated

Global Variable

# kSecTransformActionExternalizeExtraData

An action that triggers after data is stored.

macOS 10.7–13.0Deprecated

``` source
let kSecTransformActionExternalizeExtraData: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Allows for adding to the data that is stored using an override to the kSecTransformActionExternalizeExtraData block. The output of this override is a dictionary that contains the custom externalized data. A common use of this override is to write out a version number of a custom transform.


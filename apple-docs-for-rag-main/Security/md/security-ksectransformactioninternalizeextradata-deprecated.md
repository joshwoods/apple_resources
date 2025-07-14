

- Security
-  kSecTransformActionInternalizeExtraData Deprecated

Global Variable

# kSecTransformActionInternalizeExtraData

An action that triggers after attributes are read into a transform.

macOS 10.7–13.0Deprecated

``` source
let kSecTransformActionInternalizeExtraData: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Overrides the standard processing that occurs when externalized data is used to create a transform. This is closely tied to the kSecTransformActionExternalizeExtraData override. The ‘normal’ attributes are read into the new transform and then this is called to read in the items that were written out using kSecTransformActionExternalizeExtraData override. A common use of this override would be to read in the version number of the externalized custom transform.


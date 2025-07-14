

- Security
-  kSecTransformActionFinalize Deprecated

Global Variable

# kSecTransformActionFinalize

An action that triggers just before deleting a custom transform to enable custom cleanup operations.

macOS 10.7–13.0Deprecated

``` source
let kSecTransformActionFinalize: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Overrides the standard behavior that occurs just before deleting a custom transform. This is typically overridden to allow for memory clean up of a custom transform. This is used with the SecTransformOverrideTransformAction block.


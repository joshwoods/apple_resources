

- Security
-  kSecTransformActionStartingExecution Deprecated

Global Variable

# kSecTransformActionStartingExecution

An action that triggers just before starting execution of a custom transform.

macOS 10.7–13.0Deprecated

``` source
let kSecTransformActionStartingExecution: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Overrides the standard behavior that occurs just before starting execution of a custom transform. This is typically overridden to allow for initialization. This is used with the SecTransformOverrideTransformAction block.




- Security
-  kSecTransformAbortOriginatorKey 

Global Variable

# kSecTransformAbortOriginatorKey

The key in an error’s `userInfo` dictionary whose value indicates the transform that caused the chain to abort.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecTransformAbortOriginatorKey: CFString
```

## Discussion

Use the value associated with this key to determine exactly which transform failed when more than one error occurs during transform evaluation.


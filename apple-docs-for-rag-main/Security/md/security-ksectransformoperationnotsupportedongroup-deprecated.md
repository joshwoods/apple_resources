

- Security
-  kSecTransformOperationNotSupportedOnGroup Deprecated

Global Variable

# kSecTransformOperationNotSupportedOnGroup

An illegal action on a group transform has occurred.

macOS 10.7–13.0Deprecated

``` source
var kSecTransformOperationNotSupportedOnGroup: CFIndex { get }
```

## Discussion

This might happen, for example, if you call SecTransformSetAttribute(_:_:_:_:) on a group.


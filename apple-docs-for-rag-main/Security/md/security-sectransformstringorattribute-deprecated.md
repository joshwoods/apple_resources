

- Security
-  SecTransformStringOrAttribute Deprecated

Type Alias

# SecTransformStringOrAttribute

A type that may be either a string or an attribute reference.

macOS 10.7–13.0Deprecated

``` source
typealias SecTransformStringOrAttribute = CFTypeRef
```

Deprecated

SecTransform is no longer supported

## Discussion

Use a value of this type in place of either a CFString or a SecTransformAttribute when referring to transform attributes, such as with the `attribute` parameter in calls to the SecTransformCustomSetAttribute(_:_:_:_:) and SecTransformCustomGetAttribute(_:_:_:) functions. When using a name, see Transform Attributes for a list of valid key names.


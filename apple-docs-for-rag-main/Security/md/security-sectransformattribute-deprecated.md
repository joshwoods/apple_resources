

- Security
-  SecTransformAttribute Deprecated

Type Alias

# SecTransformAttribute

A direct reference to a security transform attribute.

macOS 10.7–13.0Deprecated

``` source
typealias SecTransformAttribute = CFTypeRef
```

Deprecated

SecTransform is no longer supported

## Discussion

Using an attribute reference rather than referring to it by name, such as in calls to the SecTransformCustomSetAttribute(_:_:_:_:) function, speeds up the operation.




- Security
-  SecTransformGetAttribute(\_:\_:) Deprecated

Function

# SecTransformGetAttribute(\_:\_:)

Gets the current value of a transform attribute.

macOS 10.7–12.0Deprecated

``` source
func SecTransformGetAttribute(
    _ transformRef: SecTransform,
    _ key: CFString
) -> CFTypeRef?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`transformRef`  

The transform whose attribute value will be retrieved.

`key`  

The name of the attribute to retrieve. See Transform Attributes for a list of valid keys.

## Return Value

The value of an attribute. If this attribute is being set as the output of another transform and SecTransformExecute(_:_:) has not been called on the transform or if the attribute does not exists then `NULL` will be returned.

## Discussion

This may be called after SecTransformExecute(_:_:).


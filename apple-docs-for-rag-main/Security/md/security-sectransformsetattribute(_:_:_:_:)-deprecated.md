

- Security
-  SecTransformSetAttribute(\_:\_:\_:\_:) Deprecated

Function

# SecTransformSetAttribute(\_:\_:\_:\_:)

Sets a static value for an attribute in a transform.

macOS 10.7–12.0Deprecated

``` source
func SecTransformSetAttribute(
    _ transformRef: SecTransform,
    _ key: CFString,
    _ value: CFTypeRef,
    _ error: UnsafeMutablePointer?>?
) -> Bool
```

Deprecated

SecTransform is no longer supported

## Parameters 

`transformRef`  

The transform whose attribute is to be set.

`key`  

The name of the attribute to be set. See Transform Attributes for a list of valid keys and possible values.

`value`  

The static value to set for the named attribute.

`error`  

A pointer that the function uses to provide an error object with details if an error occurs. The caller becomes responsible for the object’s memory. Pass `NULL` to ignore the error.

## Return Value

A Boolean set to true if the call succeeds. Otherwise, the `error` parameter contains information about the failure.

## Discussion

This function is useful for things like iteration counts and other non-changing values. It returns an error and the named attribute is not changed if SecTransformExecute(_:_:) has already been called on the transform.

Compare this function with the SecTransformConnectTransforms(_:_:_:_:_:_:) function which sets derived data.


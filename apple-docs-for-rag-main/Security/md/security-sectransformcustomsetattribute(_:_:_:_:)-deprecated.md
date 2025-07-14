

- Security
-  SecTransformCustomSetAttribute(\_:\_:\_:\_:) Deprecated

Function

# SecTransformCustomSetAttribute(\_:\_:\_:\_:)

Sets an attribute value on a custom transform.

macOS 10.7–13.0Deprecated

``` source
func SecTransformCustomSetAttribute(
    _ ref: SecTransformImplementationRef,
    _ attribute: SecTransformStringOrAttribute,
    _ type: SecTransformMetaAttributeType,
    _ value: CFTypeRef?
) -> CFTypeRef?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`ref`  

A SecTransformImplementationRef that is bound to an instance of a custom transform.

`attribute`  

The name or the attribute handle of the attribute whose value is to be set. When using a name, see Transform Attributes for a list of valid key names.

`type`  

The type of data to be retrieved for the attribute. See the discussion on SecTransformMetaAttributeType for details.

`value`  

The new value for the attribute

## Return Value

An error on failure, or `NULL` on success. In Objective-C, call the CFRelease function to free the error’s memory when you are done with it.

## Discussion

Unlike the SecTransformSetAttribute(_:_:_:_:) function this function can set attribute values while a transform is executing. These values are limited to the custom transform instance that is bound to the `ref` parameter.


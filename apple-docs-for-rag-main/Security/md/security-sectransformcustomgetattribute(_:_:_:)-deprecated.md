

- Security
-  SecTransformCustomGetAttribute(\_:\_:\_:) Deprecated

Function

# SecTransformCustomGetAttribute(\_:\_:\_:)

Gets an attribute value from a custom transform.

macOS 10.7–13.0Deprecated

``` source
func SecTransformCustomGetAttribute(
    _ ref: SecTransformImplementationRef,
    _ attribute: SecTransformStringOrAttribute,
    _ type: SecTransformMetaAttributeType
) -> CFTypeRef?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`ref`  

A SecTransformImplementationRef that is bound to an instance of a custom transform.

`attribute`  

The name or the attribute handle of the attribute whose value is to be retrieved. When using a name, see Transform Attributes for a list of valid key names.

`type`  

The type of data to be retrieved for the attribute. See the discussion on SecTransformMetaAttributeType for details.

## Return Value

The value of the attribute.


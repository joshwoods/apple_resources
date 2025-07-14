

- Security
-  SecTransformPushbackAttribute(\_:\_:\_:) Deprecated

Function

# SecTransformPushbackAttribute(\_:\_:\_:)

Pushes a single value back for a specific attribute.

macOS 10.7–13.0Deprecated

``` source
func SecTransformPushbackAttribute(
    _ ref: SecTransformImplementationRef,
    _ attribute: SecTransformStringOrAttribute,
    _ value: CFTypeRef
) -> CFTypeRef?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`ref`  

A SecTransformImplementationRef that is bound to an instance of a custom transform.

`attribute`  

The name or the attribute handle of the attribute whose value is to be pushed back. When using a name, see Transform Attributes for a list of valid key names.

`value`  

The value being pushed back.

## Return Value

An error on failure, or `NULL` on success. In Objective-C, call the CFRelease function to free the error’s memory when you are done with it.

## Discussion

Calling this function stops the flow of data into the specified attribute until any attribute is changed for the transform instance bound to the `ref` parameter.


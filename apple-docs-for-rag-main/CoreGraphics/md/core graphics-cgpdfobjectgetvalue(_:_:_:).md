

- Core Graphics
-  CGPDFObjectGetValue(\_:\_:\_:) 

Function

# CGPDFObjectGetValue(\_:\_:\_:)

Returns whether an object is of a given type and if it is, retrieves its value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFObjectGetValue(
    _ object: CGPDFObjectRef,
    _ type: CGPDFObjectType,
    _ value: UnsafeMutableRawPointer?
) -> Bool
```

## Parameters 

`object`  

A PDF object.

`type`  

A PDF object type.

`value`  

If the `object` parameter is a PDF object of the specified type, then on return contains that object, otherwise the value is unspecified.

## Return Value

Returns true if the specified object is a PDF object of the specified type, otherwise false.

## Discussion

The function gets the value of the `object` parameter. If the type of `object` is equal to the type specified, then:

- If the `value` parameter is not a null pointer, then the value of `object` is copied to `value`, and the function returns true.

- If the `value` parameter is a null pointer, then the function simply returns true. This allows you to test whether `object` is of the type specified.

If the type of `object` is CGPDFObjectType.integer and `type` is equal to CGPDFObjectType.real, then the value of `object` is converted to floating point, the result copied to `value`, and the function returns true. If none of the preceding conditions is met, returns false.

## See Also

### Getting Object Types and Values

func CGPDFObjectGetType(CGPDFObjectRef) -> CGPDFObjectType

Returns the PDF type identifier of an object.




- Core Graphics
-  CGPDFObjectGetType(\_:) 

Function

# CGPDFObjectGetType(\_:)

Returns the PDF type identifier of an object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFObjectGetType(_ object: CGPDFObjectRef) -> CGPDFObjectType
```

## Parameters 

`object`  

A PDF object. If the value if not a PDF object, the behavior is unspecified.

## Return Value

Returns the type of the `object` parameter. See Abstract Types for PDF Document Content.

## See Also

### Getting Object Types and Values

func CGPDFObjectGetValue(CGPDFObjectRef, CGPDFObjectType, UnsafeMutableRawPointer?) -> Bool

Returns whether an object is of a given type and if it is, retrieves its value.


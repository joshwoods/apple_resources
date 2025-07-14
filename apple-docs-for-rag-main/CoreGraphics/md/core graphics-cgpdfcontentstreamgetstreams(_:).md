

- Core Graphics
-  CGPDFContentStreamGetStreams(\_:) 

Function

# CGPDFContentStreamGetStreams(\_:)

Gets the array of PDF content streams contained in a PDF content stream object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFContentStreamGetStreams(_ cs: CGPDFContentStreamRef) -> CFArray?
```

## Parameters 

`cs`  

A PDF content stream object.

## Return Value

The array of PDF content streams that make up the content stream object represented by the `cs` parameter.

## See Also

### Getting Data from a PDF Content Stream Object

func CGPDFContentStreamGetResource(CGPDFContentStreamRef, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>) -> CGPDFObjectRef?

Gets the specified resource from a PDF content stream object.


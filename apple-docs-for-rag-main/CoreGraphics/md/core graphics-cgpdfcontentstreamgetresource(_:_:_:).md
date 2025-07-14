

- Core Graphics
-  CGPDFContentStreamGetResource(\_:\_:\_:) 

Function

# CGPDFContentStreamGetResource(\_:\_:\_:)

Gets the specified resource from a PDF content stream object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFContentStreamGetResource(
    _ cs: CGPDFContentStreamRef,
    _ category: UnsafePointer,
    _ name: UnsafePointer
) -> CGPDFObjectRef?
```

## Parameters 

`cs`  

A PDF content stream object.

`category`  

A string that specifies the category of the resource you want to obtain.

`name`  

A string that specifies the name of the resource you want to obtain.

## Return Value

The resource dictionary.

## Discussion

You can use this function to obtain resources used by the content stream, such as forms, patterns, color spaces, and fonts.

## See Also

### Getting Data from a PDF Content Stream Object

func CGPDFContentStreamGetStreams(CGPDFContentStreamRef) -> CFArray?

Gets the array of PDF content streams contained in a PDF content stream object.


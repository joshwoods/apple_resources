

- Core Graphics
-  CGPDFContentStreamCreateWithStream(\_:\_:\_:) 

Function

# CGPDFContentStreamCreateWithStream(\_:\_:\_:)

Creates a PDF content stream object from an existing PDF content stream object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFContentStreamCreateWithStream(
    _ stream: CGPDFStreamRef,
    _ streamResources: CGPDFDictionaryRef,
    _ parent: CGPDFContentStreamRef
) -> CGPDFContentStreamRef
```

## Parameters 

`stream`  

The PDF stream you want to create a content stream from.

`streamResources`  

A PDF dictionary that contains the resources associated with the stream you want to retrieve.

`parent`  

The content stream of the page on which `stream` appears. Supply the `parent` parameter when you create a content stream that’s used within a page.

## Return Value

A PDF content stream object created from the `stream` parameter. In Objective-C, you’re responsible for releasing this object by calling the CGPDFContentStreamRelease(_:) function.

## Discussion

You can use this function to get access to the contents of a form, pattern, Type3 font, or any PDF stream.

## See Also

### Creating a PDF Content Stream Object

func CGPDFContentStreamCreateWithPage(CGPDFPage) -> CGPDFContentStreamRef

Creates a content stream object from a PDF page object.


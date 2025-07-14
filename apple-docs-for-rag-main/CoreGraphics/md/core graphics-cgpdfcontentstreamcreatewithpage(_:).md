

- Core Graphics
-  CGPDFContentStreamCreateWithPage(\_:) 

Function

# CGPDFContentStreamCreateWithPage(\_:)

Creates a content stream object from a PDF page object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFContentStreamCreateWithPage(_ page: CGPDFPage) -> CGPDFContentStreamRef
```

## Parameters 

`page`  

A PDF page object.

## Return Value

A new CGPDFContentStreamRef object. In Objective-C, you’re responsible for releasing this object by calling the CGPDFContentStreamRelease(_:) function.

## Discussion

A CGPDFContentStreamRef object can contain more than one PDF content stream. To retrieve an array of the PDF content streams in the object, call the function CGPDFContentStreamGetStreams(_:). To obtain the resources associated with a CGPDFContentStreamRef object, call the function CGPDFContentStreamGetResource(_:_:_:).

## See Also

### Creating a PDF Content Stream Object

func CGPDFContentStreamCreateWithStream(CGPDFStreamRef, CGPDFDictionaryRef, CGPDFContentStreamRef) -> CGPDFContentStreamRef

Creates a PDF content stream object from an existing PDF content stream object.


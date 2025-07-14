

- Core Graphics
- CGContext
-  addDocumentMetadata(\_:) 

Instance Method

# addDocumentMetadata(\_:)

Associates custom metadata with the PDF document.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func addDocumentMetadata(_ metadata: CFData?)
```

## Parameters 

`metadata`  

A stream of XML data that is formatted according to the Extensible Metadata Platform, as described in section 10.2.2., “Metadata Streams”, of the PDF 1.7 specification.

## See Also

### Managing a PDF Graphics Context

func beginPDFPage(CFDictionary?)

Begins a new page in a PDF graphics context.

func endPDFPage()

Ends the current page in the PDF graphics context.

func addDestination(CFString, at: CGPoint)

Sets a destination to jump to when a point in the current page of a PDF graphics context is clicked.

func setDestination(CFString, for: CGRect)

Sets a destination to jump to when a rectangle in the current PDF page is clicked.

func setURL(CFURL, for: CGRect)

Sets the URL associated with a rectangle in a PDF graphics context.

func closePDF()

Closes a PDF document.


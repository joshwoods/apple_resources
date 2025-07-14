

- Core Graphics
- CGContext
-  beginPDFPage(\_:) 

Instance Method

# beginPDFPage(\_:)

Begins a new page in a PDF graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func beginPDFPage(_ pageInfo: CFDictionary?)
```

## Parameters 

`pageInfo`  

A dictionary that contains key-value pairs that define the page properties.

## Discussion

You must call the function endPDFPage() to signal the end of the page.

## See Also

### Managing a PDF Graphics Context

func endPDFPage()

Ends the current page in the PDF graphics context.

func addDestination(CFString, at: CGPoint)

Sets a destination to jump to when a point in the current page of a PDF graphics context is clicked.

func setDestination(CFString, for: CGRect)

Sets a destination to jump to when a rectangle in the current PDF page is clicked.

func setURL(CFURL, for: CGRect)

Sets the URL associated with a rectangle in a PDF graphics context.

func addDocumentMetadata(CFData?)

Associates custom metadata with the PDF document.

func closePDF()

Closes a PDF document.


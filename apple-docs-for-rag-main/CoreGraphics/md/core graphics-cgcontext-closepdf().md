

- Core Graphics
- CGContext
-  closePDF() 

Instance Method

# closePDF()

Closes a PDF document.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func closePDF()
```

## Discussion

After closing the context, all pending data is written to the context destination, and the PDF file is completed. No additional data can be written to the destination context after the PDF document is closed.

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

func addDocumentMetadata(CFData?)

Associates custom metadata with the PDF document.


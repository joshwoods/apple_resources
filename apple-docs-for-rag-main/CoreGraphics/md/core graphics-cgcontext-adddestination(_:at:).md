

- Core Graphics
- CGContext
-  addDestination(\_:at:) 

Instance Method

# addDestination(\_:at:)

Sets a destination to jump to when a point in the current page of a PDF graphics context is clicked.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func addDestination(
    _ name: CFString,
    at point: CGPoint
)
```

## Parameters 

`name`  

A destination name.

`point`  

A location in the current page of the PDF graphics context.

## See Also

### Managing a PDF Graphics Context

func beginPDFPage(CFDictionary?)

Begins a new page in a PDF graphics context.

func endPDFPage()

Ends the current page in the PDF graphics context.

func setDestination(CFString, for: CGRect)

Sets a destination to jump to when a rectangle in the current PDF page is clicked.

func setURL(CFURL, for: CGRect)

Sets the URL associated with a rectangle in a PDF graphics context.

func addDocumentMetadata(CFData?)

Associates custom metadata with the PDF document.

func closePDF()

Closes a PDF document.




- Core Graphics
- CGContext
-  setDestination(\_:for:) 

Instance Method

# setDestination(\_:for:)

Sets a destination to jump to when a rectangle in the current PDF page is clicked.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setDestination(
    _ name: CFString,
    for rect: CGRect
)
```

## Parameters 

`name`  

A destination name.

`rect`  

A rectangle that specifies an area of the current page of a PDF graphics context. The rectangle is specified in default user space (not device space).

## See Also

### Managing a PDF Graphics Context

func beginPDFPage(CFDictionary?)

Begins a new page in a PDF graphics context.

func endPDFPage()

Ends the current page in the PDF graphics context.

func addDestination(CFString, at: CGPoint)

Sets a destination to jump to when a point in the current page of a PDF graphics context is clicked.

func setURL(CFURL, for: CGRect)

Sets the URL associated with a rectangle in a PDF graphics context.

func addDocumentMetadata(CFData?)

Associates custom metadata with the PDF document.

func closePDF()

Closes a PDF document.


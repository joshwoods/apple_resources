

- Core Graphics
- CGContext
-  setURL(\_:for:) 

Instance Method

# setURL(\_:for:)

Sets the URL associated with a rectangle in a PDF graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setURL(
    _ url: CFURL,
    for rect: CGRect
)
```

## Parameters 

`url`  

A URL that specifies the destination of the contents associated with the rectangle.

`rect`  

A rectangle specified in default user space (not device space).

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

func addDocumentMetadata(CFData?)

Associates custom metadata with the PDF document.

func closePDF()

Closes a PDF document.


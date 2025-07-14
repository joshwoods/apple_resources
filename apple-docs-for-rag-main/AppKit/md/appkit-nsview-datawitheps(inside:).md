

- AppKit
- NSView
-  dataWithEPS(inside:) 

Instance Method

# dataWithEPS(inside:)

Returns EPS data that draws the region of the view within a specified rectangle.

macOS

``` source
@MainActor
func dataWithEPS(inside rect: NSRect) -> Data
```

## Parameters 

`rect`  

A rectangle defining the region.

## Discussion

This data can be placed on an NSPasteboard object, written to a file, or used to create an NSImage object.

## See Also

### Printing the View’s Content

func printView(Any?)

This action method opens the Print panel, and if the user chooses an option other than canceling, prints the view and all its subviews to the device specified in the Print panel.

func beginPage(in: NSRect, atPlacement: NSPoint)

Called at the beginning of each page, this method sets up the coordinate system so that a region inside the view’s bounds is translated to a specified location.

func dataWithPDF(inside: NSRect) -> Data

Returns PDF data that draws the region of the view within a specified rectangle.

var printJobTitle: String

The view’s print job title.

var pageHeader: NSAttributedString

A default header string that includes the print job title and date.

var pageFooter: NSAttributedString

A default footer string that includes the current page number and page count.

func writeEPS(inside: NSRect, to: NSPasteboard)

Writes EPS data that draws the region of the view within a specified rectangle onto a pasteboard.

func writePDF(inside: NSRect, to: NSPasteboard)

Writes PDF data that draws the region of the view within a specified rectangle onto a pasteboard.

func drawPageBorder(with: NSSize)

Allows applications that use the AppKit pagination facility to draw additional marks on each logical page.

func drawSheetBorder(with: NSSize)

Allows applications that use the AppKit pagination facility to draw additional marks on each printed sheet.

Deprecated


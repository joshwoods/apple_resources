

- AppKit
- NSView
-  drawSheetBorder(with:) Deprecated

Instance Method

# drawSheetBorder(with:)

Allows applications that use the AppKit pagination facility to draw additional marks on each printed sheet.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func drawSheetBorder(with borderSize: NSSize)
```

Deprecated

This is never invoked and the NSView implementation does nothing

## Parameters 

`borderSize`  

An `NSSize` structure that defines a printed sheet.

## Discussion

The marks can be such things as crop marks or fold lines of size `borderSize`. This method has been deprecated.

## See Also

### Printing the View’s Content

func printView(Any?)

This action method opens the Print panel, and if the user chooses an option other than canceling, prints the view and all its subviews to the device specified in the Print panel.

func beginPage(in: NSRect, atPlacement: NSPoint)

Called at the beginning of each page, this method sets up the coordinate system so that a region inside the view’s bounds is translated to a specified location.

func dataWithEPS(inside: NSRect) -> Data

Returns EPS data that draws the region of the view within a specified rectangle.

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


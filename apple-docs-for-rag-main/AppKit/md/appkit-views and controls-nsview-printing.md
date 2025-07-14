

- AppKit
- Views and Controls
- NSView
-  Printing 

API Collection

# Printing

Create a printable version of your view’s content and handle pagination and printer-related behaviors.

## Topics

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

func drawSheetBorder(with: NSSize)

Allows applications that use the AppKit pagination facility to draw additional marks on each printed sheet.

Deprecated

### Handling Pagination

var heightAdjustLimit: CGFloat

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as lines of text from being divided across pages.

var widthAdjustLimit: CGFloat

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as small images or text columns from being divided across pages.

func adjustPageWidthNew(UnsafeMutablePointer&lt;CGFloat>, left: CGFloat, right: CGFloat, limit: CGFloat)

Overridden by subclasses to adjust page width during automatic pagination.

func adjustPageHeightNew(UnsafeMutablePointer&lt;CGFloat>, top: CGFloat, bottom: CGFloat, limit: CGFloat)

Overridden by subclasses to adjust page height during automatic pagination.

func knowsPageRange(NSRangePointer) -> Bool

Returns true if the view handles page boundaries, false otherwise.

func rectForPage(Int) -> NSRect

Implemented by subclasses to determine the portion of the view to be printed for the specified page number.

func locationOfPrintRect(NSRect) -> NSPoint

Invoked by printView(_:) to determine the location of the region of the view being printed on the physical page.

### Writing Conforming Rendering Instructions

func beginDocument()

Invoked at the beginning of the printing session, this method sets up the current graphics context.

func endDocument()

This method is invoked at the end of the printing session.

func endPage()

Writes the end of a conforming page.

## See Also

### Managing the view’s content

Layout

Specify the size and position your view relative to other nearby views using rules that update your view hierarchy automatically.

Drawing

Draw the content of custom views and update that content when the view’s size or appearance changes.


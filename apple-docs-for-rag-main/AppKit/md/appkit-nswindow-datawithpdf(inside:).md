

- AppKit
- NSWindow
-  dataWithPDF(inside:) 

Instance Method

# dataWithPDF(inside:)

Returns PDF data that draws the region of the window within a given rectangle.

macOS

``` source
@MainActor
func dataWithPDF(inside rect: NSRect) -> Data
```

## Parameters 

`rect`  

A rectangle (expressed in the window’s coordinate system) that identifies the region to be expressed as PDF data.

## Return Value

The region in the window (identified by `rect`) as PDF data.

## Discussion

This data can be placed on a pasteboard, written to a file, or used to create an `NSImage` object.

## See Also

### Related Documentation

func writePDF(inside: NSRect, to: NSPasteboard)

Writes PDF data that draws the region of the view within a specified rectangle onto a pasteboard.

func dataWithPDF(inside: NSRect) -> Data

Returns PDF data that draws the region of the view within a specified rectangle.

### Printing Windows

func printWindow(Any?)

Runs the Print panel, and if the user chooses an option other than canceling, prints the window (its frame view and all subviews).

func dataWithEPS(inside: NSRect) -> Data

Returns EPS data that draws the region of the window within a given rectangle.




- AppKit
- NSWindow
-  dataWithEPS(inside:) 

Instance Method

# dataWithEPS(inside:)

Returns EPS data that draws the region of the window within a given rectangle.

macOS

``` source
@MainActor
func dataWithEPS(inside rect: NSRect) -> Data
```

## Parameters 

`rect`  

A rectangle (expressed in the window’s coordinate system) that identifies the region to be expressed as EPS data.

## Return Value

The region in the window (identified by `rect`) as EPS data.

## Discussion

This data can be placed on a pasteboard, written to a file, or used to create an `NSImage` object.

## See Also

### Related Documentation

func dataWithEPS(inside: NSRect) -> Data

Returns EPS data that draws the region of the view within a specified rectangle.

func writeEPS(inside: NSRect, to: NSPasteboard)

Writes EPS data that draws the region of the view within a specified rectangle onto a pasteboard.

### Printing Windows

func printWindow(Any?)

Runs the Print panel, and if the user chooses an option other than canceling, prints the window (its frame view and all subviews).

func dataWithPDF(inside: NSRect) -> Data

Returns PDF data that draws the region of the window within a given rectangle.


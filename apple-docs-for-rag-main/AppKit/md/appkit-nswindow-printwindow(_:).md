

- AppKit
- NSWindow
-  printWindow(\_:) 

Instance Method

# printWindow(\_:)

Runs the Print panel, and if the user chooses an option other than canceling, prints the window (its frame view and all subviews).

macOS

``` source
@MainActor
func printWindow(_ sender: Any?)
```

## Parameters 

`sender`  

The message’s sender.

## See Also

### Printing Windows

func dataWithEPS(inside: NSRect) -> Data

Returns EPS data that draws the region of the window within a given rectangle.

func dataWithPDF(inside: NSRect) -> Data

Returns PDF data that draws the region of the window within a given rectangle.


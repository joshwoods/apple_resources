

- AppKit
- NSBrowserCell
-  isLeaf 

Instance Property

# isLeaf

A Boolean that indicates whether the browser cell is a leaf or a branch cell.

macOS

``` source
@MainActor
var isLeaf: Bool { get set }
```

## Discussion

When the value of this property is true, the browser cell is a leaf cell.

A branch `NSBrowserCell` has an image near its right edge indicating that more, hierarchically related information is available; when the user selects the cell, the `NSBrowser` displays a new column of `NSBrowserCell` objects. A leaf `NSBrowserCell` has no image, indicating that the user has reached a terminal piece of information; it doesn’t point to additional information.

## See Also

### Managing Browser Cell State

func reset()

Unhighlights the receiver and unsets its state.

func set()

Highlights the receiver and sets its state.

var isLoaded: Bool

A Boolean that indicates whether the cell is ready to display.

func highlightColor(in: NSView) -> NSColor?

Returns the highlight color that the receiver wants to display.


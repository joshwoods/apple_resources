

- AppKit
- NSBrowserCell
-  isLoaded 

Instance Property

# isLoaded

A Boolean that indicates whether the cell is ready to display.

macOS

``` source
@MainActor
var isLoaded: Bool { get set }
```

## Discussion

When the value of this property is true, the browser cell’s state has been set and the cell is ready to display.

## See Also

### Managing Browser Cell State

func reset()

Unhighlights the receiver and unsets its state.

func set()

Highlights the receiver and sets its state.

var isLeaf: Bool

A Boolean that indicates whether the browser cell is a leaf or a branch cell.

func highlightColor(in: NSView) -> NSColor?

Returns the highlight color that the receiver wants to display.


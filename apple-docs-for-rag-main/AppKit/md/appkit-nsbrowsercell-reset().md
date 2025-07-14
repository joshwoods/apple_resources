

- AppKit
- NSBrowserCell
-  reset() 

Instance Method

# reset()

Unhighlights the receiver and unsets its state.

macOS

``` source
@MainActor
func reset()
```

## See Also

### Managing Browser Cell State

func set()

Highlights the receiver and sets its state.

var isLeaf: Bool

A Boolean that indicates whether the browser cell is a leaf or a branch cell.

var isLoaded: Bool

A Boolean that indicates whether the cell is ready to display.

func highlightColor(in: NSView) -> NSColor?

Returns the highlight color that the receiver wants to display.


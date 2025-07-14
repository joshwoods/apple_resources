

- AppKit
- NSBrowserCell
-  set() 

Instance Method

# set()

Highlights the receiver and sets its state.

macOS

``` source
@MainActor
func set()
```

## See Also

### Managing Browser Cell State

func reset()

Unhighlights the receiver and unsets its state.

var isLeaf: Bool

A Boolean that indicates whether the browser cell is a leaf or a branch cell.

var isLoaded: Bool

A Boolean that indicates whether the cell is ready to display.

func highlightColor(in: NSView) -> NSColor?

Returns the highlight color that the receiver wants to display.


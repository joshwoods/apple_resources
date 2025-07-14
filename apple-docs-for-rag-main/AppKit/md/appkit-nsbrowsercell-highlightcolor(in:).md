

- AppKit
- NSBrowserCell
-  highlightColor(in:) 

Instance Method

# highlightColor(in:)

Returns the highlight color that the receiver wants to display.

macOS

``` source
@MainActor
func highlightColor(in controlView: NSView) -> NSColor?
```

## Parameters 

`controlView`  

The view for which to return the highlight color.

## Return Value

The highlight color.

## See Also

### Managing Browser Cell State

func reset()

Unhighlights the receiver and unsets its state.

func set()

Highlights the receiver and sets its state.

var isLeaf: Bool

A Boolean that indicates whether the browser cell is a leaf or a branch cell.

var isLoaded: Bool

A Boolean that indicates whether the cell is ready to display.


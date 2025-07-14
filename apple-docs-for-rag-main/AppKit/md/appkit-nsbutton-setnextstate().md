

- AppKit
- NSButton
-  setNextState() 

Instance Method

# setNextState()

Sets the button to its next state.

macOS

``` source
@MainActor
func setNextState()
```

## Discussion

If the button has three states, it cycles through them in this order: on, off, mixed, on, and so forth. If the button has two states, it toggles between them.

## See Also

### Managing Button State

var allowsMixedState: Bool

A Boolean value that indicates whether the button allows a mixed state.

var state: NSControl.StateValue

The button’s state.

func highlight(Bool)

Highlights (or unhighlights) the button.


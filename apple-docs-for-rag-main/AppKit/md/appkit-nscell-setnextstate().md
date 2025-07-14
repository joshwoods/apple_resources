

- AppKit
- NSCell
-  setNextState() 

Instance Method

# setNextState()

Changes cell’s state to the next value in the sequence.

macOS

``` source
@MainActor
func setNextState()
```

## Discussion

If a cell has three states, it cycles in this order: on, off, mixed, on, off, and so forth. If the cell has only two states, it toggles between them.

## See Also

### Managing Cell State

var allowsMixedState: Bool

A Boolean value indicating whether the cell supports three states instead of two.

var nextState: Int

The cell’s next state.

var state: NSControl.StateValue

The cell’s current state.

struct StateValue

A constant that indicates whether a control is on, off, or in a mixed state.


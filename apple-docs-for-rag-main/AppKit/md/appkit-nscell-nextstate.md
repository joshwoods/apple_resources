

- AppKit
- NSCell
-  nextState 

Instance Property

# nextState

The cell’s next state.

macOS

``` source
@MainActor
var nextState: Int { get }
```

## Discussion

If a cell has three states, it cycles in this order: on, off, mixed, on, off, and so forth. If the cell has only two states, it toggles between them.

For a list of constants representing the possible cell states, see NSCell.StateValue.

## See Also

### Managing Cell State

var allowsMixedState: Bool

A Boolean value indicating whether the cell supports three states instead of two.

func setNextState()

Changes cell’s state to the next value in the sequence.

var state: NSControl.StateValue

The cell’s current state.

struct StateValue

A constant that indicates whether a control is on, off, or in a mixed state.


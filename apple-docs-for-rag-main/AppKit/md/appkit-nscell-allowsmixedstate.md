

- AppKit
- NSCell
-  allowsMixedState 

Instance Property

# allowsMixedState

A Boolean value indicating whether the cell supports three states instead of two.

macOS

``` source
@MainActor
var allowsMixedState: Bool { get set }
```

## Discussion

When the value of this property is true, the cell supports three states: on, off, and mixed. When the value is false, the cell supports only the on and off states.

## See Also

### Managing Cell State

var nextState: Int

The cell’s next state.

func setNextState()

Changes cell’s state to the next value in the sequence.

var state: NSControl.StateValue

The cell’s current state.

struct StateValue

A constant that indicates whether a control is on, off, or in a mixed state.


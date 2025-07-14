

- AppKit
- NSCell
-  state 

Instance Property

# state

The cell’s current state.

macOS

``` source
@MainActor
var state: NSControl.StateValue { get set }
```

## Discussion

The NSOffState state indicates the normal or unpressed state. The NSOnState state indicates the alternate or pressed state. The NSMixedState state indicates that the feature represented by the control is in effect somewhere.

Although using the enumerated constants is preferred, you can also assign an integer value to this property. If the cell has two states, `0` is treated as NSOffState, and a nonzero value is treated as NSOnState. If the cell has three states, `0` is treated as NSOffState, a negative value is treated as `NSMixedState`, and a positive value is treated as NSOnState.

## See Also

### Managing Cell State

var allowsMixedState: Bool

A Boolean value indicating whether the cell supports three states instead of two.

var nextState: Int

The cell’s next state.

func setNextState()

Changes cell’s state to the next value in the sequence.

struct StateValue

A constant that indicates whether a control is on, off, or in a mixed state.


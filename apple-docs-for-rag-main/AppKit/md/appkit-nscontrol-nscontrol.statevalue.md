

- AppKit
- NSControl
-  NSControl.StateValue 

Structure

# NSControl.StateValue

A constant that indicates whether a control is on, off, or in a mixed state.

macOS

``` source
struct StateValue
```

## Topics

### Setting a Control’s State

static let on: NSControl.StateValue

A constant value that indicates a control is on or selected.

static let off: NSControl.StateValue

A constant value that indicates a control is off or unselected.

static let mixed: NSControl.StateValue

A constant value that indicates a control is in a mixed state, neither on nor off.

### Creating a State Value

init(Int)

Initializes a control state object.

init(rawValue: Int)

Initializes a state value from a raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Cell State

var allowsMixedState: Bool

A Boolean value indicating whether the cell supports three states instead of two.

var nextState: Int

The cell’s next state.

func setNextState()

Changes cell’s state to the next value in the sequence.

var state: NSControl.StateValue

The cell’s current state.


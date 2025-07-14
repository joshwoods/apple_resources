

- UIKit
- UIControl
-  state 

Instance Property

# state

The state of the control, specified as a bit mask value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var state: UIControl.State { get }
```

## Discussion

The value of this property is a bitmask of the constants in the UIControl.State type. A control can be in more than one state at a time. For example, it can be focused and highlighted at the same time. You can also get the values for individual states using the properties of this class.

## See Also

### Managing state

struct State

Constants describing the state of a control.

var isEnabled: Bool

A Boolean value indicating whether the control is in the enabled state.

var isSelected: Bool

A Boolean value indicating whether the control is in the selected state.

var isHighlighted: Bool

A Boolean value indicating whether the control draws a highlight.


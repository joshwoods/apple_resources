

- UIKit
- UIControl
-  isEnabled 

Instance Property

# isEnabled

A Boolean value indicating whether the control is in the enabled state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

Set the value of this property to true to enable the control or false to disable it. An enabled control is capable of responding to user interactions, whereas a disabled control ignores touch events and may draw itself differently. Setting this property to false adds the disabled flag to the control’s state bitmask; enabling the control again removes that flag.

The default value of this property is true for a newly created control. You can set a control’s initial enabled state in your storyboard file.

## See Also

### Managing state

var state: UIControl.State

The state of the control, specified as a bit mask value.

struct State

Constants describing the state of a control.

var isSelected: Bool

A Boolean value indicating whether the control is in the selected state.

var isHighlighted: Bool

A Boolean value indicating whether the control draws a highlight.


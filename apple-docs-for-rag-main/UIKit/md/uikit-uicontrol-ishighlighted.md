

- UIKit
- UIControl
-  isHighlighted 

Instance Property

# isHighlighted

A Boolean value indicating whether the control draws a highlight.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isHighlighted: Bool { get set }
```

## Discussion

When the value of this property is true, the control draws a highlight; otherwise, the control doesn’t draw a highlight. Controls automatically set and clear this state in response to appropriate touch events. You can change the value of this property as needed to apply or remove a highlight programmatically

The default value of this property is false for a newly created control. You can set a control’s initial selected state in your storyboard file.

## See Also

### Managing state

var state: UIControl.State

The state of the control, specified as a bit mask value.

struct State

Constants describing the state of a control.

var isEnabled: Bool

A Boolean value indicating whether the control is in the enabled state.

var isSelected: Bool

A Boolean value indicating whether the control is in the selected state.


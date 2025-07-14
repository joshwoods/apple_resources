

- UIKit
- UIControl
-  isSelected 

Instance Property

# isSelected

A Boolean value indicating whether the control is in the selected state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isSelected: Bool { get set }
```

## Discussion

Set the value of this property to true to select it or false to deselect it. Most controls don’t modify their appearance or behavior when selected, but some do. For example, the UISegmentedControl class tracks whether a segment is selected and draws it differently when it is.

The default value of this property is false for a newly created control. You can set a control’s initial selected state in your storyboard file.

## See Also

### Managing state

var state: UIControl.State

The state of the control, specified as a bit mask value.

struct State

Constants describing the state of a control.

var isEnabled: Bool

A Boolean value indicating whether the control is in the enabled state.

var isHighlighted: Bool

A Boolean value indicating whether the control draws a highlight.


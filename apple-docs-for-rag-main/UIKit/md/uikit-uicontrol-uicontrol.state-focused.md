

- UIKit
- UIControl
- UIControl.State
-  focused 

Type Property

# focused

The focused state of a control.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
static var focused: UIControl.State { get }
```

## Discussion

In focus-based navigation systems, a control enters this state when it receives the focus. A focused control changes its appearance to indicate that it has focus, and this appearance differs from the appearance of the control when it’s highlighted or selected. Further interactions with the control can result in it also becoming highlighted or selected.

## See Also

### Constants

static var normal: UIControl.State

The normal, or default, state of a control where the control is enabled but neither selected nor highlighted.

static var highlighted: UIControl.State

The highlighted state of a control.

static var disabled: UIControl.State

The disabled state of a control.

static var selected: UIControl.State

The selected state of a control.

static var application: UIControl.State

Additional control-state flags available for app use.

static var reserved: UIControl.State

Control-state flags reserved for internal framework use.




- UIKit
- UIControl
- UIControl.State
-  highlighted 

Type Property

# highlighted

The highlighted state of a control.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
static var highlighted: UIControl.State { get }
```

## Discussion

A control becomes highlighted when a touch event enters the control’s bounds, and it loses that highlight when there’s a touch-up event or when the touch event exits the control’s bounds. You can retrieve and set this value through the isHighlighted property.

## See Also

### Constants

static var normal: UIControl.State

The normal, or default, state of a control where the control is enabled but neither selected nor highlighted.

static var disabled: UIControl.State

The disabled state of a control.

static var selected: UIControl.State

The selected state of a control.

static var focused: UIControl.State

The focused state of a control.

static var application: UIControl.State

Additional control-state flags available for app use.

static var reserved: UIControl.State

Control-state flags reserved for internal framework use.




- UIKit
- UIControl
- UIControl.State
-  disabled 

Type Property

# disabled

The disabled state of a control.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
static var disabled: UIControl.State { get }
```

## Discussion

User interactions with disabled control have no effect and the control draws itself with a dimmed appearance to reflect that it’s disabled. You can retrieve and set this value through the isEnabled property.

## See Also

### Constants

static var normal: UIControl.State

The normal, or default, state of a control where the control is enabled but neither selected nor highlighted.

static var highlighted: UIControl.State

The highlighted state of a control.

static var selected: UIControl.State

The selected state of a control.

static var focused: UIControl.State

The focused state of a control.

static var application: UIControl.State

Additional control-state flags available for app use.

static var reserved: UIControl.State

Control-state flags reserved for internal framework use.


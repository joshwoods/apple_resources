

- UIKit
- UIControl
- UIControl.State
-  selected 

Type Property

# selected

The selected state of a control.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
static var selected: UIControl.State { get }
```

## Discussion

For many controls, this state has no effect on behavior or appearance. Some subclasses, like the UISegmentedControl class, use this state to change their appearance. You can retrieve and set this value through the isSelected property.

## See Also

### Constants

static var normal: UIControl.State

The normal, or default, state of a control where the control is enabled but neither selected nor highlighted.

static var highlighted: UIControl.State

The highlighted state of a control.

static var disabled: UIControl.State

The disabled state of a control.

static var focused: UIControl.State

The focused state of a control.

static var application: UIControl.State

Additional control-state flags available for app use.

static var reserved: UIControl.State

Control-state flags reserved for internal framework use.


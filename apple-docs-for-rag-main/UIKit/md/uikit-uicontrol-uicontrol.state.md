

- UIKit
- UIControl
-  UIControl.State 

Structure

# UIControl.State

Constants describing the state of a control.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct State
```

## Overview

A control can have more than one state at a time. Controls can have different configurations according to their state. For example, a UIButton object can display one image when it’s in its normal state and a different image when it’s highlighted.

## Topics

### Constants

static var normal: UIControl.State

The normal, or default, state of a control where the control is enabled but neither selected nor highlighted.

static var highlighted: UIControl.State

The highlighted state of a control.

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

### Initializers

init(rawValue: UInt)

Creates a control state with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing state

var state: UIControl.State

The state of the control, specified as a bit mask value.

var isEnabled: Bool

A Boolean value indicating whether the control is in the enabled state.

var isSelected: Bool

A Boolean value indicating whether the control is in the selected state.

var isHighlighted: Bool

A Boolean value indicating whether the control draws a highlight.




- AppKit
- NSButton
-  NSButton.ButtonType 

Enumeration

# NSButton.ButtonType

Button types that you can specify using setButtonType(_:).

macOS

``` source
enum ButtonType
```

## Overview

For examples of how these types behave, see Button Programming Topics.

## Topics

### Configuring Button Behavior

case momentaryPushIn

A button that illuminates when the user clicks it.

case momentaryLight

A button that displays a highlight when the user clicks it and returns to its normal state when the user releases it.

case momentaryChange

A button that displays its alternate content when clicked and returns to its normal content when the user releases it.

case pushOnPushOff

A button that switches between on and off states with each click.

case onOff

A button that switches between a normal and emphasized bezel on each click.

case toggle

A button that switches between its normal and alternate content on each click.

case `switch`

A standard checkbox button.

case radio

A button that displays a single selected value from group of possible choices.

case accelerator

A button that sends repeating actions as pressure changes occur.

case multiLevelAccelerator

A button that allows for a configurable number of stepped pressure levels and provides tactile feedback as the user reaches each step.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum BezelStyle

The set of bezel styles to style buttons in your app.

enum GradientType

Specify the gradients used by the gradientType property.

Deprecated


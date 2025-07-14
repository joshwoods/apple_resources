

- AppKit
- NSButton
-  NSButton.BezelStyle 

Enumeration

# NSButton.BezelStyle

The set of bezel styles to style buttons in your app.

macOS

``` source
enum BezelStyle
```

## Overview

For design guidance on buttons, see Human Interface Guidelines > Buttons.

## Topics

### Default

case automatic

The default button style based on the button’s contents and position within the window.

### Push

case push

A standard push style button.

case flexiblePush

A push button with a flexible height to accommodate longer text labels or an image.

### Disclosure

case disclosure

A bezel style button for use with a disclosure triangle.

case pushDisclosure

A bezel style push button with a disclosure triangle.

### Toolbar

case toolbar

A button style that’s appropriate for a toolbar item.

case accessoryBar

A button style that’s typically used in the context of an accessory toolbar for buttons that narrow the focus of a search or other operation.

case accessoryBarAction

A button style that you use for extra actions in an accessory toolbar.

### Informational

case helpButton

A round button with a question mark, providing the standard help button look.

case badge

A button style suitable for displaying additional information.

case circular

A round button that can contain either a single character or an icon.

### Other

case smallSquare

A simple square bezel style that can scale to any size.

### Deprecated

Deprecated Symbols

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

enum ButtonType

Button types that you can specify using setButtonType(_:).

enum GradientType

Specify the gradients used by the gradientType property.

Deprecated


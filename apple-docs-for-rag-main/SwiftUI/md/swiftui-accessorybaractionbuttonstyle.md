

- SwiftUI
-  AccessoryBarActionButtonStyle 

Structure

# AccessoryBarActionButtonStyle

A button style that you use for extra actions in an accessory toolbar.

macOS 14.0+

``` source
struct AccessoryBarActionButtonStyle
```

## Overview

Use this style for buttons that perform extra actions relative to the accessory toolbar’s main functions, like adding or editing filters. This style also affects other view types that you apply a button style to, like Toggle, Picker, and Menu instances.

Use accessoryBarAction to construct this style.

## Topics

### Creating the button style

init()

Creates an accessory toolbar action button style

### Supporting types

func makeBody(configuration: AccessoryBarActionButtonStyle.Configuration) -> some View

Creates a view that represents the body of a button.

## Relationships

### Conforms To

- PrimitiveButtonStyle

## See Also

### Supporting types

struct DefaultButtonStyle

The default button style, based on the button’s context.

struct AccessoryBarButtonStyle

A button style that you use for actions in an accessory toolbar that narrow the focus of a search or other operation.

struct BorderedButtonStyle

A button style that applies standard border artwork based on the button’s context.

struct BorderedProminentButtonStyle

A button style that applies standard border prominent artwork based on the button’s context.

struct BorderlessButtonStyle

A button style that doesn’t apply a border.

struct CardButtonStyle

A button style that doesn’t pad the content, and applies a motion effect when a button has focus.

struct LinkButtonStyle

A button style for buttons that emulate links.

struct PlainButtonStyle

A button style that doesn’t style or decorate its content while idle, but may apply a visual effect to indicate the pressed, focused, or enabled state of the button.


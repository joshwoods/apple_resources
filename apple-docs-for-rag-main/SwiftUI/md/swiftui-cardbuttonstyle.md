

- SwiftUI
-  CardButtonStyle 

Structure

# CardButtonStyle

A button style that doesn’t pad the content, and applies a motion effect when a button has focus.

tvOS 14.0+

``` source
struct CardButtonStyle
```

## Overview

You can also use card to construct this style.

## Topics

### Creating the button style

init()

Creates a style that doesn’t pad a button’s content and applies a motion effect to a focused button.

### Supporting types

func makeBody(configuration: CardButtonStyle.Configuration) -> some View

Creates a view that represents the body of a button.

## Relationships

### Conforms To

- PrimitiveButtonStyle

## See Also

### Related Documentation

@MainActor class TVCardView

A view that responds to focus interaction with a motion effect it applies to all of its subviews.

### Supporting types

struct DefaultButtonStyle

The default button style, based on the button’s context.

struct AccessoryBarButtonStyle

A button style that you use for actions in an accessory toolbar that narrow the focus of a search or other operation.

struct AccessoryBarActionButtonStyle

A button style that you use for extra actions in an accessory toolbar.

struct BorderedButtonStyle

A button style that applies standard border artwork based on the button’s context.

struct BorderedProminentButtonStyle

A button style that applies standard border prominent artwork based on the button’s context.

struct BorderlessButtonStyle

A button style that doesn’t apply a border.

struct LinkButtonStyle

A button style for buttons that emulate links.

struct PlainButtonStyle

A button style that doesn’t style or decorate its content while idle, but may apply a visual effect to indicate the pressed, focused, or enabled state of the button.


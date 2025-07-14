

- SwiftUI
-  BorderlessButtonMenuStyle Deprecated

Structure

# BorderlessButtonMenuStyle

A menu style that displays a borderless button that toggles the display of the menu’s contents when pressed.

iOS 14.0–18.4DeprecatediPadOS 14.0–18.4DeprecatedMac Catalyst 14.0–18.4DeprecatedmacOS 11.0–15.4DeprecatedtvOS 17.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
struct BorderlessButtonMenuStyle
```

Deprecated

Use menuStyle(_:) with button and buttonStyle(_:) with borderless.

## Overview

Use borderlessButton to construct this style.

## Topics

### Creating a bordeless button menu style

init()

Creates a borderless button menu style.

init(showsMenuIndicator: Bool)

Creates a borderless button menu style, specifying whether to show a visual menu indicator.

## Relationships

### Conforms To

- MenuStyle

## See Also

### Supporting types

struct DefaultMenuStyle

The default menu style, based on the menu’s context.

struct ButtonMenuStyle

A menu style that displays a button that toggles the display of the menu’s contents when pressed.

struct BorderedButtonMenuStyle

A menu style that displays a bordered button that toggles the display of the menu’s contents when pressed.

Deprecated


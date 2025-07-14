

- SwiftUI
-  MenuStyle 

Protocol

# MenuStyle

A type that applies standard interaction behavior and a custom appearance to all menus within a view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol MenuStyle
```

## Overview

To configure the current menu style for a view hierarchy, use the menuStyle(_:) modifier.

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Getting built-in menu styles

static var automatic: DefaultMenuStyle

The default menu style, based on the menu’s context.

static var button: ButtonMenuStyle

A menu style that displays a button that toggles the display of the menu’s contents when pressed.

static var borderedButton: BorderedButtonMenuStyle

A menu style that displays a bordered button that toggles the display of the menu’s contents when pressed.

Deprecated

static var borderlessButton: BorderlessButtonMenuStyle

A menu style that displays a borderless button that toggles the display of the menu’s contents when pressed.

Deprecated

### Creating custom menu styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a menu.

**Required**

typealias Configuration

The properties of a menu.

associatedtype Body : View

A view that represents the body of a menu.

**Required**

### Supporting types

struct DefaultMenuStyle

The default menu style, based on the menu’s context.

struct ButtonMenuStyle

A menu style that displays a button that toggles the display of the menu’s contents when pressed.

struct BorderlessButtonMenuStyle

A menu style that displays a borderless button that toggles the display of the menu’s contents when pressed.

Deprecated

struct BorderedButtonMenuStyle

A menu style that displays a bordered button that toggles the display of the menu’s contents when pressed.

Deprecated

## Relationships

### Conforming Types

- BorderedButtonMenuStyle
- BorderlessButtonMenuStyle
- ButtonMenuStyle
- DefaultMenuStyle

## See Also

### Styling menus

func menuStyle&lt;S>(S) -> some View

Sets the style for menus within this view.

struct MenuStyleConfiguration

A configuration of a menu.


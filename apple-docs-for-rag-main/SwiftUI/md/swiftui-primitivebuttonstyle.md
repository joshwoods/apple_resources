

- SwiftUI
-  PrimitiveButtonStyle 

Protocol

# PrimitiveButtonStyle

A type that applies custom interaction behavior and a custom appearance to all buttons within a view hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
protocol PrimitiveButtonStyle
```

## Overview

To configure the current button style for a view hierarchy, use the buttonStyle(_:) modifier. Specify a style that conforms to `PrimitiveButtonStyle` to create a button with custom interaction behavior. To create a button with the standard button interaction behavior defined for each platform, use ButtonStyle instead.

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

### Getting built-in button styles

static var automatic: DefaultButtonStyle

The default button style, based on the button’s context.

static var accessoryBar: AccessoryBarButtonStyle

A button style that is typically used in the context of an accessory toolbar (sometimes refererred to as a “scope bar”), for buttons that narrow the focus of a search or other operation.

static var accessoryBarAction: AccessoryBarActionButtonStyle

A button style that you use for extra actions in an accessory toolbar.

static var bordered: BorderedButtonStyle

A button style that applies standard border artwork based on the button’s context.

static var borderedProminent: BorderedProminentButtonStyle

A button style that applies standard border prominent artwork based on the button’s context.

static var borderless: BorderlessButtonStyle

A button style that doesn’t apply a border.

static var card: CardButtonStyle

A button style that doesn’t pad the content, and applies a motion effect when a button has focus.

static var link: LinkButtonStyle

A button style for buttons that emulate links.

static var plain: PlainButtonStyle

A button style that doesn’t style or decorate its content while idle, but may apply a visual effect to indicate the pressed, focused, or enabled state of the button.

### Creating custom button styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a button.

**Required**

typealias Configuration

The properties of a button.

associatedtype Body : View

A view that represents the body of a button.

**Required**

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

struct CardButtonStyle

A button style that doesn’t pad the content, and applies a motion effect when a button has focus.

struct LinkButtonStyle

A button style for buttons that emulate links.

struct PlainButtonStyle

A button style that doesn’t style or decorate its content while idle, but may apply a visual effect to indicate the pressed, focused, or enabled state of the button.

## Relationships

### Conforming Types

- AccessoryBarActionButtonStyle
- AccessoryBarButtonStyle
- BorderedButtonStyle
- BorderedProminentButtonStyle
- BorderlessButtonStyle
- CardButtonStyle
- DefaultButtonStyle
- LinkButtonStyle
- PlainButtonStyle

## See Also

### Styling buttons

func buttonStyle(_:)

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

protocol ButtonStyle

A type that applies standard interaction behavior and a custom appearance to all buttons within a view hierarchy.

struct ButtonStyleConfiguration

The properties of a button.

struct PrimitiveButtonStyleConfiguration

The properties of a button.

func signInWithAppleButtonStyle(SignInWithAppleButton.Style) -> some View

Sets the style used for displaying the control (see `SignInWithAppleButton.Style`).


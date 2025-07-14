

- SwiftUI
-  ButtonStyleConfiguration 

Structure

# ButtonStyleConfiguration

The properties of a button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ButtonStyleConfiguration
```

## Topics

### Configuring a button’s label

let label: ButtonStyleConfiguration.Label

A view that describes the effect of pressing the button.

struct Label

A type-erased label of a button.

### Configuring a button’s interaction state

let isPressed: Bool

A Boolean that indicates whether the user is currently pressing the button.

### Defining the button’s purpose

let role: ButtonRole?

An optional semantic role that describes the button’s purpose.

## See Also

### Styling buttons

func buttonStyle(_:)

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

protocol ButtonStyle

A type that applies standard interaction behavior and a custom appearance to all buttons within a view hierarchy.

protocol PrimitiveButtonStyle

A type that applies custom interaction behavior and a custom appearance to all buttons within a view hierarchy.

struct PrimitiveButtonStyleConfiguration

The properties of a button.

func signInWithAppleButtonStyle(SignInWithAppleButton.Style) -> some View

Sets the style used for displaying the control (see `SignInWithAppleButton.Style`).


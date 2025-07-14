

- SwiftUI
-  ButtonStyle 

Protocol

# ButtonStyle

A type that applies standard interaction behavior and a custom appearance to all buttons within a view hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
protocol ButtonStyle
```

## Overview

To configure the current button style for a view hierarchy, use the buttonStyle(_:) modifier. Specify a style that conforms to `ButtonStyle` when creating a button that uses the standard button interaction behavior defined for each platform. To create a button with custom interaction behavior, use PrimitiveButtonStyle instead.

## Topics

### Custom button styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a button.

**Required**

typealias Configuration

The properties of a button.

associatedtype Body : View

A view that represents the body of a button.

**Required**

## See Also

### Styling buttons

func buttonStyle(_:)

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

struct ButtonStyleConfiguration

The properties of a button.

protocol PrimitiveButtonStyle

A type that applies custom interaction behavior and a custom appearance to all buttons within a view hierarchy.

struct PrimitiveButtonStyleConfiguration

The properties of a button.

func signInWithAppleButtonStyle(SignInWithAppleButton.Style) -> some View

Sets the style used for displaying the control (see `SignInWithAppleButton.Style`).




- AppKit
- NSButton
-  NSButton.GradientType Deprecated

Enumeration

# NSButton.GradientType

Specify the gradients used by the gradientType property.

macOS 10.0–10.12Deprecated

``` source
enum GradientType
```

## Topics

### Constants

case none

There is no gradient, so the button looks flat.

case concaveWeak

The top-left corner is light gray, and the bottom-right corner is dark gray, so the button appears to be pushed in.

case concaveStrong

As with `NSGradientConcaveWeak`, the top-left corner is light gray, and the bottom-right corner is dark gray, but the difference between the grays is greater, so the appearance of being pushed in is stronger.

case convexWeak

The top-left corner is dark gray, and the bottom-right corner is light gray, so the button appears to be sticking out.

case convexStrong

As with `NSGradientConvexWeak`, the top-left corner is dark gray, and the bottom-right corner is light gray, but the difference between the grays is greater, so the appearance of sticking out is stronger.

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

enum ButtonType

Button types that you can specify using setButtonType(_:).


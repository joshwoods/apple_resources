

- PassKit (Apple Pay and Wallet)
-  PKPaymentButtonStyle 

Enumeration

# PKPaymentButtonStyle

A type that indicates the available appearances for an Apple Pay button.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
enum PKPaymentButtonStyle
```

## Topics

### Payment button styles

case white

A white button with black lettering.

case whiteOutline

A white button with black lettering and a black outline.

case black

A black button with white lettering.

case automatic

A button that automatically changes its appearance when the user switches between Light Mode and Dark Mode.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the appearance

enum PKPaymentButtonType

The Apple Pay button types you can display to initiate Apple Pay transactions.

var cornerRadius: CGFloat

The radius, in points, for the rounded corners on the button.


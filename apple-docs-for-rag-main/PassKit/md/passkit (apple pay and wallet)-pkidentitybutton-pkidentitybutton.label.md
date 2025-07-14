

- PassKit (Apple Pay and Wallet)
- PKIdentityButton
-  PKIdentityButton.Label 

Enumeration

# PKIdentityButton.Label

A type that indicates the available labels for an identity button.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum Label
```

## Topics

### Labels

case verifyIdentity

A label with the text verify identity with Apple Wallet.

case verify

A label with the text verify with Apple Wallet.

case verifyAge

A label with the text verify age with Apple Wallet.

case `continue`

A label with the text continue with Apple Wallet.

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

enum Style

A type that indicates the available appearances for an identity button.

var cornerRadius: CGFloat

The radius for the rounded corners on the button, in points.


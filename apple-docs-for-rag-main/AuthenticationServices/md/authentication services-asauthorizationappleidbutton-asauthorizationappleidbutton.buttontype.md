

- Authentication Services
- ASAuthorizationAppleIDButton
-  ASAuthorizationAppleIDButton.ButtonType 

Enumeration

# ASAuthorizationAppleIDButton.ButtonType

A type for the authorization button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum ButtonType
```

## Topics

### Choosing a Button Type

case `continue`

A button type that continues the Sign in with Apple authorization process.

static var `default`: ASAuthorizationAppleIDButton.ButtonType

A default button type for the Sign in with Apple authorization process.

case signUp

A button type that allows the user to sign up for Sign in with Apple.

case signIn

A button type that performs authorization using Sign in with Apple.

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

### Styling the Button

var cornerRadius: CGFloat

The radius, in points, for the rounded corners on the Apple ID sign-in button.

enum Style

A style for the authorization button.




- Authentication Services
- SignInWithAppleButton
-  SignInWithAppleButton.Style 

Structure

# SignInWithAppleButton.Style

The structure that defines styles that you use to control the button’s appearance.

AuthenticationServicesSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct Style
```

## Topics

### Styles

static let black: SignInWithAppleButton.Style

The constant that defines a black button.

static let white: SignInWithAppleButton.Style

The constant that defines a white button.

static let whiteOutline: SignInWithAppleButton.Style

The constant that defines a white-outlined button.

## See Also

### Creating a button

init(SignInWithAppleButton.Label, onRequest: (ASAuthorizationAppleIDRequest) -> Void, onCompletion: (Result&lt;ASAuthorization, any Error>) -> Void)

Creates a Sign in with Apple button.

struct Label

The label that appears on the button.


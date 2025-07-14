

- Authentication Services
- SignInWithAppleButton
-  SignInWithAppleButton.Label 

Structure

# SignInWithAppleButton.Label

The label that appears on the button.

AuthenticationServicesSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct Label
```

## Topics

### Labels

static let `continue`: SignInWithAppleButton.Label

The constant that defines the Continue label on the button.

static let signIn: SignInWithAppleButton.Label

The constant that defines the Sign in with Apple label on the button.

static let signUp: SignInWithAppleButton.Label

The constant that defines the Sign up with Apple label on the button.

## See Also

### Creating a button

init(SignInWithAppleButton.Label, onRequest: (ASAuthorizationAppleIDRequest) -> Void, onCompletion: (Result&lt;ASAuthorization, any Error>) -> Void)

Creates a Sign in with Apple button.

struct Style

The structure that defines styles that you use to control the button’s appearance.


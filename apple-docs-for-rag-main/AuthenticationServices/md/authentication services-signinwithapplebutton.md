

- Authentication Services
-  SignInWithAppleButton 

Structure

# SignInWithAppleButton

The view that creates the Sign in with Apple button for display.

AuthenticationServicesSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
struct SignInWithAppleButton
```

## Topics

### Creating a button

init(SignInWithAppleButton.Label, onRequest: (ASAuthorizationAppleIDRequest) -> Void, onCompletion: (Result&lt;ASAuthorization, any Error>) -> Void)

Creates a Sign in with Apple button.

struct Label

The label that appears on the button.

struct Style

The structure that defines styles that you use to control the button’s appearance.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Sign In with Apple

Implementing User Authentication with Sign in with Apple

Provide a way for users of your app to set up an account and start using your services.

Simplifying User Authentication in a tvOS App

Build a fluid sign-in experience for your tvOS apps using AuthenticationServices.

Sign in with Apple Entitlement

An entitlement that lets your app use Sign in with Apple.

class ASAuthorizationAppleIDProvider

A mechanism for generating requests to authenticate users based on their Apple ID.

class ASAuthorizationAppleIDCredential

A credential that results from a successful Apple ID authentication.


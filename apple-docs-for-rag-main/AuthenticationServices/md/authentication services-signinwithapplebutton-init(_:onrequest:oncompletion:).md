

- Authentication Services
- SignInWithAppleButton
-  init(\_:onRequest:onCompletion:) 

Initializer

# init(\_:onRequest:onCompletion:)

Creates a Sign in with Apple button.

AuthenticationServicesSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    _ label: SignInWithAppleButton.Label = .signIn,
    onRequest: @escaping (ASAuthorizationAppleIDRequest) -> Void,
    onCompletion: @escaping (Result) -> Void
)
```

## Parameters 

`label`  

The label that appears on the button.

`onRequest`  

The authorization request for an Apple ID.

`onCompletion`  

The completion handler that the system calls when the sign-in completes.

## See Also

### Creating a button

struct Label

The label that appears on the button.

struct Style

The structure that defines styles that you use to control the button’s appearance.


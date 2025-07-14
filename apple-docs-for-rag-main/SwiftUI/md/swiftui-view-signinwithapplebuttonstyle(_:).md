

- SwiftUI
- View
-  signInWithAppleButtonStyle(\_:) 

Instance Method

# signInWithAppleButtonStyle(\_:)

Sets the style used for displaying the control (see `SignInWithAppleButton.Style`).

AuthenticationServicesSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func signInWithAppleButtonStyle(_ style: SignInWithAppleButton.Style) -> some View
```

## Parameters 

`style`  

The sign in style to apply to this button.

## See Also

### Authorizing and authenticating

@MainActor @preconcurrency struct LocalAuthenticationView&lt;Label> where Label : View

A SwiftUI view that displays an authentication interface.

@MainActor @preconcurrency struct SignInWithAppleButton

The view that creates the Sign in with Apple button for display.

var authorizationController: AuthorizationController

A value provided in the SwiftUI environment that views can use to perform authorization requests.

var webAuthenticationSession: WebAuthenticationSession

A value provided in the SwiftUI environment that views can use to authenticate a user through a web service.


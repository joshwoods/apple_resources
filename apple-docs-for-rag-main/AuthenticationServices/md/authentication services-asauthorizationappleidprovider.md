

- Authentication Services
-  ASAuthorizationAppleIDProvider 

Class

# ASAuthorizationAppleIDProvider

A mechanism for generating requests to authenticate users based on their Apple ID.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class ASAuthorizationAppleIDProvider
```

## Overview

You use a provider to create a request (ASAuthorizationAppleIDRequest), which you then use to initialize a controller (ASAuthorizationController) that performs the request:

```
```

On success, the controller’s delegate receives an authorization (ASAuthorization) containing a credential (ASAuthorizationAppleIDCredential) that has an opaque user identifier. You can use that identifier to later check the user’s credential state—for example, to see if authorization has been revoked—by calling the getCredentialState(forUserID:completion:) method:

```
```

## Topics

### Offering Sign In with Apple

class ASAuthorizationAppleIDButton

A control you add to your interface that enables users to initiate the Sign In with Apple flow.

class WKInterfaceAuthorizationAppleIDButton

A button that you can use to trigger a Sign in with Apple request.

### Creating Requests

func createRequest() -> ASAuthorizationAppleIDRequest

Creates a new Apple ID authorization request.

class ASAuthorizationAppleIDRequest

An OpenID authorization request that relies on the user’s Apple ID.

class ASAuthorizationOpenIDRequest

An OpenID authorization request.

### Getting State

func getCredentialState(forUserID: String, completion: (ASAuthorizationAppleIDProvider.CredentialState, (any Error)?) -> Void)

Returns the credential state for the given user in a completion handler.

enum CredentialState

Possible values for the credential state of a user.

class let credentialRevokedNotification: NSNotification.Name

A notification that indicates the user’s credentials have been revoked and they should be signed out.

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationProvider
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Sign In with Apple

Implementing User Authentication with Sign in with Apple

Provide a way for users of your app to set up an account and start using your services.

Simplifying User Authentication in a tvOS App

Build a fluid sign-in experience for your tvOS apps using AuthenticationServices.

struct SignInWithAppleButton

The view that creates the Sign in with Apple button for display.

Sign in with Apple Entitlement

An entitlement that lets your app use Sign in with Apple.

class ASAuthorizationAppleIDCredential

A credential that results from a successful Apple ID authentication.


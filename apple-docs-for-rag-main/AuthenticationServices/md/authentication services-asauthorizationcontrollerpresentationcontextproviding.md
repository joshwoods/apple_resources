

- Authentication Services
-  ASAuthorizationControllerPresentationContextProviding 

Protocol

# ASAuthorizationControllerPresentationContextProviding

An interface the controller uses to ask a delegate for a presentation context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
protocol ASAuthorizationControllerPresentationContextProviding : NSObjectProtocol
```

## Mentioned in 

Authenticating people by using passkeys in browser apps

## Topics

### Specifying the Anchor

func presentationAnchor(for: ASAuthorizationController) -> ASPresentationAnchor

Tells the delegate from which window it should present content to the user.

**Required**

typealias ASPresentationAnchor

A platform-specific type that indicates the kind of user interface element to use as a presentation anchor.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Presenting requests

var presentationContextProvider: (any ASAuthorizationControllerPresentationContextProviding)?

A delegate that provides a display context in which the system can present an authorization interface to the user.


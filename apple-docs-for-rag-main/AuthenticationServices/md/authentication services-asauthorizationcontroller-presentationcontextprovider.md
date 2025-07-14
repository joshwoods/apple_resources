

- Authentication Services
- ASAuthorizationController
-  presentationContextProvider 

Instance Property

# presentationContextProvider

A delegate that provides a display context in which the system can present an authorization interface to the user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
weak var presentationContextProvider: (any ASAuthorizationControllerPresentationContextProviding)? { get set }
```

## See Also

### Presenting requests

protocol ASAuthorizationControllerPresentationContextProviding

An interface the controller uses to ask a delegate for a presentation context.


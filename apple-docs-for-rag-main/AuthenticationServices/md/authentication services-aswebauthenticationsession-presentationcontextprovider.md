

- Authentication Services
- ASWebAuthenticationSession
-  presentationContextProvider 

Instance Property

# presentationContextProvider

A delegate that provides a display context in which the system can present an authentication session to the user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
weak var presentationContextProvider: (any ASWebAuthenticationPresentationContextProviding)? { get set }
```

## Mentioned in 

Authenticating a User Through a Web Service

## See Also

### Presenting a Session

protocol ASWebAuthenticationPresentationContextProviding

An interface the session uses to ask a delegate for a presentation context.


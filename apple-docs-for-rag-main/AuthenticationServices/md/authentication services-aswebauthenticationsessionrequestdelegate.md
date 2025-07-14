

- Authentication Services
-  ASWebAuthenticationSessionRequestDelegate 

Protocol

# ASWebAuthenticationSessionRequestDelegate

An interface through which the session request can inform its delegate, which is typically a browser, about the outcome of the authentication attempt.

macOS 10.15+

``` source
protocol ASWebAuthenticationSessionRequestDelegate : NSObjectProtocol
```

## Topics

### Responding to Completion Events

func authenticationSessionRequest(ASWebAuthenticationSessionRequest, didCompleteWithCallbackURL: URL)

Tells the delegate, typically a browser, that the authentication completed successfully.

func authenticationSessionRequest(ASWebAuthenticationSessionRequest, didCancelWithError: any Error)

Tells the delegate, typically a browser, that the authentication was canceled.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Indicating Completion

var delegate: (any ASWebAuthenticationSessionRequestDelegate)?

A delegate that the session request instance informs about authentication completion.


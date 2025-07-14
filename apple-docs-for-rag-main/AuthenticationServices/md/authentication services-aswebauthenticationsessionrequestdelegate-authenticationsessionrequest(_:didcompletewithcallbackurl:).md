

- Authentication Services
- ASWebAuthenticationSessionRequestDelegate
-  authenticationSessionRequest(\_:didCompleteWithCallbackURL:) 

Instance Method

# authenticationSessionRequest(\_:didCompleteWithCallbackURL:)

Tells the delegate, typically a browser, that the authentication completed successfully.

macOS 10.15+

``` source
optional func authenticationSessionRequest(
    _ authenticationSessionRequest: ASWebAuthenticationSessionRequest,
    didCompleteWithCallbackURL callbackURL: URL
)
```

## Parameters 

`authenticationSessionRequest`  

The request sending the message.

`callbackURL`  

A URL using the scheme indicated by the request’s callbackURLScheme property that indicates the outcome of the authentication attempt.

## See Also

### Responding to Completion Events

func authenticationSessionRequest(ASWebAuthenticationSessionRequest, didCancelWithError: any Error)

Tells the delegate, typically a browser, that the authentication was canceled.


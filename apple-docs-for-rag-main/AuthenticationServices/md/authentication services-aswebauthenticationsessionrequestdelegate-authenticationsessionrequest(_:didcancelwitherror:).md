

- Authentication Services
- ASWebAuthenticationSessionRequestDelegate
-  authenticationSessionRequest(\_:didCancelWithError:) 

Instance Method

# authenticationSessionRequest(\_:didCancelWithError:)

Tells the delegate, typically a browser, that the authentication was canceled.

macOS 10.15+

``` source
optional func authenticationSessionRequest(
    _ authenticationSessionRequest: ASWebAuthenticationSessionRequest,
    didCancelWithError error: any Error
)
```

## Parameters 

`authenticationSessionRequest`  

The request sending the message.

`error`  

An error that indicates the reason for the cancelation.

## See Also

### Responding to Completion Events

func authenticationSessionRequest(ASWebAuthenticationSessionRequest, didCompleteWithCallbackURL: URL)

Tells the delegate, typically a browser, that the authentication completed successfully.


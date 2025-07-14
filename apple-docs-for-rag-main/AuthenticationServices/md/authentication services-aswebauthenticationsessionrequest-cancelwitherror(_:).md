

- Authentication Services
- ASWebAuthenticationSessionRequest
-  cancelWithError(\_:) 

Instance Method

# cancelWithError(\_:)

Indicates that the browser canceled the authentication attempt.

macOS 10.15+

``` source
func cancelWithError(_ error: any Error)
```

## Parameters 

`error`  

An error with domain ASWebAuthenticationSessionErrorDomain and a suitable code from ASWebAuthenticationSessionError.Code that indicates the reason for the cancelation.

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## Discussion

Call this method from your browser app when the authentication attempt fails to complete, for example because the user cancels it.

## See Also

### Finishing a Request

func complete(withCallbackURL: URL)

Indicates that the browser successfully completed the authentication attempt.


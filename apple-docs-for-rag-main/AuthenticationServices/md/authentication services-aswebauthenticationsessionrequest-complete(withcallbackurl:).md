

- Authentication Services
- ASWebAuthenticationSessionRequest
-  complete(withCallbackURL:) 

Instance Method

# complete(withCallbackURL:)

Indicates that the browser successfully completed the authentication attempt.

macOS 10.15+

``` source
func complete(withCallbackURL url: URL)
```

## Parameters 

`url`  

A URL using the scheme indicated by the request’s callbackURLScheme property that indicates the outcome of the authentication attempt.

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## Discussion

Call this method from your browser app when the authentication attempt completes to report the result of the attempt using the callback URL.

## See Also

### Finishing a Request

func cancelWithError(any Error)

Indicates that the browser canceled the authentication attempt.




- Authentication Services
- ASWebAuthenticationSessionWebBrowserSessionHandling
-  cancel(\_:) 

Instance Method

# cancel(\_:)

Cancels the process of handling the given request.

macOS 10.15+

``` source
func cancel(_ request: ASWebAuthenticationSessionRequest!)
```

**Required**

## Parameters 

`request`  

The request to cancel.

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## Discussion

Your browser app implements this method to accept cancellation requests from the initiating app.

When you’ve finished your app’s teardown activities in your implementation of this method, call cancelWithError(_:) on the provided request object. Use ASWebAuthenticationSessionErrorDomain for the error domain and ASWebAuthenticationSessionError.Code.canceledLogin for the error code, unless another error happened that you need to communicate to the system.

## See Also

### Starting and Stopping a Session Request

func begin(ASWebAuthenticationSessionRequest!)

Handles the given session request from an app.

**Required**

class ASWebAuthenticationSessionRequest

A login session request that a web browser receives from an app.


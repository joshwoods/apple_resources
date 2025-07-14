

- Authentication Services
- ASWebAuthenticationSessionWebBrowserSessionHandling
-  begin(\_:) 

Instance Method

# begin(\_:)

Handles the given session request from an app.

macOS 10.15+

``` source
func begin(_ request: ASWebAuthenticationSessionRequest!)
```

**Required**

## Parameters 

`request`  

The request to begin handling.

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## Discussion

Your browser app implements this method to accept requests from apps that want to use single sign-on for authentication. Inspect the given request to see what URL to use for the request, and what call back scheme to use to reply to the app. Call the request’s complete(withCallbackURL:) method to indicate a completed authentication. Call the cancelWithError(_:) method if the browser can’t complete the operation, for example because the user cancels it.

## See Also

### Starting and Stopping a Session Request

func cancel(ASWebAuthenticationSessionRequest!)

Cancels the process of handling the given request.

**Required**

class ASWebAuthenticationSessionRequest

A login session request that a web browser receives from an app.


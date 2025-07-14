

- Authentication Services
-  ASWebAuthenticationSessionWebBrowserSessionHandling 

Protocol

# ASWebAuthenticationSessionWebBrowserSessionHandling

An interface that a session handler implements to handle login requests from an app.

macOS 10.15+

``` source
protocol ASWebAuthenticationSessionWebBrowserSessionHandling
```

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## Topics

### Starting and Stopping a Session Request

func begin(ASWebAuthenticationSessionRequest!)

Handles the given session request from an app.

**Required**

func cancel(ASWebAuthenticationSessionRequest!)

Cancels the process of handling the given request.

**Required**

class ASWebAuthenticationSessionRequest

A login session request that a web browser receives from an app.

## See Also

### Handling a Session Request

var sessionHandler: any ASWebAuthenticationSessionWebBrowserSessionHandling

A handler that a web browser provides to handle session requests from an app.


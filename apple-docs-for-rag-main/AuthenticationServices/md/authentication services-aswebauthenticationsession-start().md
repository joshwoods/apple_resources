

- Authentication Services
- ASWebAuthenticationSession
-  start() 

Instance Method

# start()

Starts a web authentication session.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.15+tvOS 16.0+visionOS 1.0+watchOS 6.2+

``` source
func start() -> Bool
```

## Return Value

A Boolean value indicating whether the web authentication session started successfully.

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

Authenticating a User Through a Web Service

## Discussion

Only call this method once for a given ASWebAuthenticationSession instance after initialization. Calling the start() method on a canceled session results in a failure.

In macOS, and for iOS apps with a deployment target of iOS 13 or later, after you call start(), the session instance stores a strong reference to itself. To avoid deallocation during the authentication process, the session keeps the reference until after it calls the completion handler.

For iOS apps with a deployment target earlier than iOS 13, your app must keep a strong reference to the session to prevent the system from deallocating the session while waiting for authentication to complete.

## See Also

### Starting and Stopping a Session

var canStart: Bool

A Boolean indicating whether the session can begin.

func cancel()

Cancels a web authentication session.


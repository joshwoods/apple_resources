

- Foundation
- URLSession
-  init(configuration:delegate:delegateQueue:) 

Initializer

# init(configuration:delegate:delegateQueue:)

Creates a session with the specified session configuration, delegate, and operation queue.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    configuration: URLSessionConfiguration,
    delegate: (any URLSessionDelegate)?,
    delegateQueue queue: OperationQueue?
)
```

## Parameters 

`configuration`  

A configuration object that specifies certain behaviors, such as caching policies, timeouts, proxies, pipelining, TLS versions to support, cookie policies, and credential storage.

See URLSessionConfiguration for more information.

`delegate`  

A session delegate object that handles requests for authentication and other session-related events.

This delegate object is responsible for handling authentication challenges, for making caching decisions, and for handling other session-related events. If `nil`, the class should be used only with methods that take completion handlers.

Important

The session object keeps a strong reference to the delegate until your app exits or explicitly invalidates the session. If you do not invalidate the session by calling the invalidateAndCancel() or finishTasksAndInvalidate() method, your app leaks memory until it exits.

`queue`  

An operation queue for scheduling the delegate calls and completion handlers. The queue should be a serial queue, in order to ensure the correct ordering of callbacks. If `nil`, the session creates a serial operation queue for performing all delegate method calls and completion handler calls.

## Mentioned in 

Fetching website data into memory

## See Also

### Creating a session

init(configuration: URLSessionConfiguration)

Creates a session with the specified session configuration.

class URLSessionConfiguration

A configuration object that defines behavior and policies for a URL session.

var configuration: URLSessionConfiguration

A copy of the configuration object for this session.


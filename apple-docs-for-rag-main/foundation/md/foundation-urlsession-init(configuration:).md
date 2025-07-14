

- Foundation
- URLSession
-  init(configuration:) 

Initializer

# init(configuration:)

Creates a session with the specified session configuration.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(configuration: URLSessionConfiguration)
```

## Parameters 

`configuration`  

A configuration object that specifies certain behaviors, such as caching policies, timeouts, proxies, pipelining, TLS versions to support, cookie policies, credential storage, and so on.

See URLSessionConfiguration for more information.

## Discussion

Calling this method is equivalent to calling init(configuration:delegate:delegateQueue:) with a `nil` delegate and queue.

## See Also

### Creating a session

init(configuration: URLSessionConfiguration, delegate: (any URLSessionDelegate)?, delegateQueue: OperationQueue?)

Creates a session with the specified session configuration, delegate, and operation queue.

class URLSessionConfiguration

A configuration object that defines behavior and policies for a URL session.

var configuration: URLSessionConfiguration

A copy of the configuration object for this session.


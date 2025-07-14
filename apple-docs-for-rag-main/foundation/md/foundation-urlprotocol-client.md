

- Foundation
- URLProtocol
-  client 

Instance Property

# client

The object the protocol uses to communicate with the URL loading system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var client: (any URLProtocolClient)? { get }
```

## See Also

### Getting protocol attributes

var cachedResponse: CachedURLResponse?

The protocol’s cached response.

protocol URLProtocolClient

The interface used by URLProtocol subclasses to communicate with the URL Loading System.

var request: URLRequest

The protocol’s request.

var task: URLSessionTask?

The protocol’s task.


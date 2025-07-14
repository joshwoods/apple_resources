

- Foundation
- URLProtocol
-  task 

Instance Property

# task

The protocol’s task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var task: URLSessionTask? { get }
```

## See Also

### Getting protocol attributes

var cachedResponse: CachedURLResponse?

The protocol’s cached response.

var client: (any URLProtocolClient)?

The object the protocol uses to communicate with the URL loading system.

protocol URLProtocolClient

The interface used by URLProtocol subclasses to communicate with the URL Loading System.

var request: URLRequest

The protocol’s request.




- Foundation
- URLProtocol
-  cachedResponse 

Instance Property

# cachedResponse

The protocol’s cached response.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var cachedResponse: CachedURLResponse? { get }
```

## Discussion

If not overridden in a subclass, this method returns the cached response stored at initialization time.

## See Also

### Getting protocol attributes

var client: (any URLProtocolClient)?

The object the protocol uses to communicate with the URL loading system.

protocol URLProtocolClient

The interface used by URLProtocol subclasses to communicate with the URL Loading System.

var request: URLRequest

The protocol’s request.

var task: URLSessionTask?

The protocol’s task.




- Foundation
- URLProtocol
-  init(task:cachedResponse:client:) 

Initializer

# init(task:cachedResponse:client:)

Creates a URL protocol instance to handle the task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    task: URLSessionTask,
    cachedResponse: CachedURLResponse?,
    client: (any URLProtocolClient)?
)
```

## Parameters 

`task`  

A task containing a URL request to be performed by the protocol.

`cachedResponse`  

A cached response for the task; may be `nil` if there is no existing cached response for the task.

`client`  

An object that provides an implementation of the URLProtocolClient protocol that this instance uses to communicate with the URL loading system. This client object is retained.

## Return Value

The initialized protocol object.

## Discussion

Subclasses should override this method to do any custom initialization. Don’t call this method explicitly. When you register your custom protocol class, the system will initialize instances of your protocol as needed.

This initializer calls through to init(request:cachedResponse:client:).

## See Also

### Creating protocol objects

init(request: URLRequest, cachedResponse: CachedURLResponse?, client: (any URLProtocolClient)?)

Creates a URL protocol instance to handle the request.


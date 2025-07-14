

- Foundation
- URLProtocol
-  init(request:cachedResponse:client:) 

Initializer

# init(request:cachedResponse:client:)

Creates a URL protocol instance to handle the request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    request: URLRequest,
    cachedResponse: CachedURLResponse?,
    client: (any URLProtocolClient)?
)
```

## Parameters 

`request`  

The URL request for the URL protocol object. This request is retained.

`cachedResponse`  

A cached response for the request; it may be `nil` if there is no existing cached response for the request.

`client`  

An object that provides an implementation of the URLProtocolClient protocol that this instance uses to communicate with the URL Loading System. This client object is retained.

## Return Value

The initialized protocol object.

## Discussion

Subclasses should override this method to do any custom initialization. Don’t call this method explicitly. When you register your custom protocol class, the system will initialize instances of your protocol as needed.

This is the designated initializer for URLProtocol.

## See Also

### Creating protocol objects

convenience init(task: URLSessionTask, cachedResponse: CachedURLResponse?, client: (any URLProtocolClient)?)

Creates a URL protocol instance to handle the task.


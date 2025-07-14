

- SMS and Call Reporting
- ILMessageFilterQueryHandling
-  handle(\_:context:completion:) 

Instance Method

# handle(\_:context:completion:)

Evaluates a query request and tells the system how to handle the message represented in the request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
func handle(
    _ queryRequest: ILMessageFilterQueryRequest,
    context: ILMessageFilterExtensionContext,
    completion: @escaping (ILMessageFilterQueryResponse) -> Void
)
```

``` source
func handle(
    _ queryRequest: ILMessageFilterQueryRequest,
    context: ILMessageFilterExtensionContext
) async -> ILMessageFilterQueryResponse
```

**Required**

## Parameters 

`queryRequest`  

A query request that describes a received message.

`context`  

The app extension context that defines APIs to defer the request to a server, if necessary.

`completion`  

A completion block used to return a response that describes how to handle the message. You can invoke this block asynchronously.


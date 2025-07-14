

- Foundation
- URLSessionTaskDelegate
-  urlSession(\_:task:willBeginDelayedRequest:completionHandler:) 

Instance Method

# urlSession(\_:task:willBeginDelayedRequest:completionHandler:)

Tells the delegate that a delayed URL session task will now begin loading.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func urlSession(
    _ session: URLSession,
    task: URLSessionTask,
    willBeginDelayedRequest request: URLRequest,
    completionHandler: @escaping (URLSession.DelayedRequestDisposition, URLRequest?) -> Void
)
```

``` source
optional func urlSession(
    _ session: URLSession,
    task: URLSessionTask,
    willBeginDelayedRequest request: URLRequest
) async -> (URLSession.DelayedRequestDisposition, URLRequest?)
```

## Parameters 

`session`  

The session containing the delayed request.

`task`  

The task handling the delayed request.

`request`  

The request that was delayed.

`completionHandler`  

A completion handler to perform the request. The completion handler takes two parameters: a disposition that tells the task how to proceed, and a new request object that is only used if the disposition is URLSession.DelayedRequestDisposition.useNewRequest.

## Discussion

This method is called when a background session task with a delayed start time (as set with the earliestBeginDate property) is ready to start. This delegate method should only be implemented if the request might become stale while waiting for the network load and needs to be replaced by a new request.

For loading to continue, the delegate must call the completion handler, passing in a disposition that indicates how the task should proceed. Passing the URLSession.DelayedRequestDisposition.cancel disposition is equivalent to calling cancel() on the task directly.

## See Also

### Handling delayed and waiting tasks

enum DelayedRequestDisposition

The action to take on a delayed URL session task.

func urlSession(URLSession, taskIsWaitingForConnectivity: URLSessionTask)

Tells the delegate that the task is waiting until suitable connectivity is available before beginning the network load.


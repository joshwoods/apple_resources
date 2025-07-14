

- Foundation
- URLSession
-  URLSession.DelayedRequestDisposition 

Enumeration

# URLSession.DelayedRequestDisposition

The action to take on a delayed URL session task.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum DelayedRequestDisposition
```

## Overview

The values of this enumeration indicate how to handle a task with a delayed start time (as set with the earliestBeginDate property). When the task is ready to start, it calls the urlSession(_:task:willBeginDelayedRequest:completionHandler:) method of URLSessionTaskDelegate. The implementation of this method must call the provided completion handler, passing in one case of this enumeration as the first argument. If the URLSession.DelayedRequestDisposition.useNewRequest disposition is used for the first argument, the caller must also provide a new NSURLRequest as the second argument.

## Topics

### Dispositions

case cancel

A disposition indicating that the task should be canceled.

case continueLoading

A disposition indicating that the task should proceed with the original request.

case useNewRequest

A disposition indicating that the task should use a new request to perform the network load.

case cancel

A disposition indicating that the task should be canceled.

case continueLoading

A disposition indicating that the task should proceed with the original request.

case useNewRequest

A disposition indicating that the task should use a new request to perform the network load.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling delayed and waiting tasks

func urlSession(URLSession, task: URLSessionTask, willBeginDelayedRequest: URLRequest, completionHandler: (URLSession.DelayedRequestDisposition, URLRequest?) -> Void)

Tells the delegate that a delayed URL session task will now begin loading.

func urlSession(URLSession, taskIsWaitingForConnectivity: URLSessionTask)

Tells the delegate that the task is waiting until suitable connectivity is available before beginning the network load.


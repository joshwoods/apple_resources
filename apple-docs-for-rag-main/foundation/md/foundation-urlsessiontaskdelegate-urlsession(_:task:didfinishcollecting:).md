

- Foundation
- URLSessionTaskDelegate
-  urlSession(\_:task:didFinishCollecting:) 

Instance Method

# urlSession(\_:task:didFinishCollecting:)

Tells the delegate that the session finished collecting metrics for the task.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
optional func urlSession(
    _ session: URLSession,
    task: URLSessionTask,
    didFinishCollecting metrics: URLSessionTaskMetrics
)
```

## Parameters 

`session`  

The session collecting the metrics.

`task`  

The task whose metrics have been collected.

`metrics`  

The collected metrics.

## See Also

### Collecting task metrics

class URLSessionTaskMetrics

An object encapsulating the metrics for a session task.


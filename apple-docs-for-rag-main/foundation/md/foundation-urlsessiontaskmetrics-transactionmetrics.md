

- Foundation
- URLSessionTaskMetrics
-  transactionMetrics 

Instance Property

# transactionMetrics

An array of metrics for each individual request-response transaction made during the execution of the task.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var transactionMetrics: [URLSessionTaskTransactionMetrics] { get }
```

## See Also

### Accessing task metrics

class URLSessionTaskTransactionMetrics

An object that encapsualtes the performance metrics collected by the URL Loading System during the execution of a session task.

var taskInterval: DateInterval

The time interval between when a task is instantiated and when the task is completed.

var redirectCount: Int

The number of redirects that occurred during the execution of the task.


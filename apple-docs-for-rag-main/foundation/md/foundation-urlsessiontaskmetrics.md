

- Foundation
-  URLSessionTaskMetrics 

Class

# URLSessionTaskMetrics

An object encapsulating the metrics for a session task.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class URLSessionTaskMetrics
```

## Overview

Each URLSessionTaskMetrics object contains the taskInterval and redirectCount, as well as metrics for each request-and-response transaction made during the execution of the task.

## Topics

### Creating task metrics

init()

Creates a task metrics instance.

Deprecated

### Accessing task metrics

var transactionMetrics: [URLSessionTaskTransactionMetrics]

An array of metrics for each individual request-response transaction made during the execution of the task.

class URLSessionTaskTransactionMetrics

An object that encapsualtes the performance metrics collected by the URL Loading System during the execution of a session task.

var taskInterval: DateInterval

The time interval between when a task is instantiated and when the task is completed.

var redirectCount: Int

The number of redirects that occurred during the execution of the task.

### Type Methods

class func new() -> SelfDeprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Collecting task metrics

func urlSession(URLSession, task: URLSessionTask, didFinishCollecting: URLSessionTaskMetrics)

Tells the delegate that the session finished collecting metrics for the task.


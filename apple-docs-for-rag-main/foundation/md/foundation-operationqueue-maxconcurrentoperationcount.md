

- Foundation
- OperationQueue
-  maxConcurrentOperationCount 

Instance Property

# maxConcurrentOperationCount

The maximum number of queued operations that can run at the same time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maxConcurrentOperationCount: Int { get set }
```

## Discussion

The value in this property affects only the operations that the current queue has executing at the same time. Other operation queues can also execute their maximum number of operations in parallel.

Reducing the number of concurrent operations does not affect any operations that are currently executing. Specifying the value `NSOperationQueueDefaultMaxConcurrentOperationCount` (which is recommended) causes the system to set the maximum number of operations based on system conditions.

The default value of this property is defaultMaxConcurrentOperationCount. You may monitor changes to the value of this property using Key-value observing. Configure an observer to monitor the maxConcurrentOperationCount key path of the operation queue.

## See Also

### Managing the Execution of Operations

var qualityOfService: QualityOfService

The default service level to apply to operations that the queue invokes.

class let defaultMaxConcurrentOperationCount: Int

The default maximum number of operations to invoke concurrently in a queue.




- Foundation
- OperationQueue
-  defaultMaxConcurrentOperationCount 

Type Property

# defaultMaxConcurrentOperationCount

The default maximum number of operations to invoke concurrently in a queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let defaultMaxConcurrentOperationCount: Int
```

## Discussion

The operation queue determines this number dynamically based on current system conditions.

## See Also

### Managing the Execution of Operations

var qualityOfService: QualityOfService

The default service level to apply to operations that the queue invokes.

var maxConcurrentOperationCount: Int

The maximum number of queued operations that can run at the same time.


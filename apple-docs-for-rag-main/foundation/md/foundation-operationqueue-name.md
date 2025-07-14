

- Foundation
- OperationQueue
-  name 

Instance Property

# name

The name of the operation queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String? { get set }
```

## Discussion

Names provide a way for you to identify your operation queues at run time. Tools may also use this name to provide additional context during debugging or analysis of your code.

The default value of this property is a string containing the memory address of the operation queue. You may monitor changes to the value of this property using Key-value observing. Configure an observer to monitor the name key path of the operation queue.

## See Also

### Configuring the Queue

var underlyingQueue: dispatch_queue_t?

The dispatch queue that the operation queue uses to invoke operations.




- Foundation
- OperationQueue
-  underlyingQueue 

Instance Property

# underlyingQueue

The dispatch queue that the operation queue uses to invoke operations.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var underlyingQueue: dispatch_queue_t? { get set }
```

## Discussion

The default value of this property is `nil`. You can set the value of this property to an existing dispatch queue to have enqueued operations interspersed with blocks submitted to that dispatch queue.

The value of this property should only be set if there are no operations in the queue; setting the value of this property when operationCount is not equal to `0` raises an invalidArgumentException. The value of this property must not be the value returned by dispatch_get_main_queue. The quality-of-service level set for the underlying dispatch queue overrides any value set for the operation queue’s qualityOfService property.

Note

This property automatically retains its assigned queue if `OS_OBJECT_IS_OBJC` is true.

## See Also

### Configuring the Queue

var name: String?

The name of the operation queue.




- Foundation
- Operation
-  threadPriority Deprecated

Instance Property

# threadPriority

The thread priority to use when executing the operation

iOS 4.0–8.0DeprecatediPadOS 4.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var threadPriority: Double { get set }
```

Deprecated

Use qualityOfService instead.

## See Also

### Configuring the Execution Priority

var qualityOfService: QualityOfService

The relative amount of importance for granting system resources to the operation.

var queuePriority: Operation.QueuePriority

The execution priority of the operation in an operation queue.


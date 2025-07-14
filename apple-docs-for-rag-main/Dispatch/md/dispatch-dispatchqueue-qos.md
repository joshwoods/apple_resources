

- Dispatch
- DispatchQueue
-  qos 

Instance Property

# qos

The quality-of-service level assgined to the queue.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
var qos: DispatchQoS { get }
```

## See Also

### Managing Queue Attributes

var label: String

The label you assigned to the dispatch queue at creation time.

func setTarget(queue: dispatch_queue_t?)

Specifies the dispatch queue on which to perform work associated with the current object.


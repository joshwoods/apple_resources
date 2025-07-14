

- Dispatch
- DispatchQueue
-  label 

Instance Property

# label

The label you assigned to the dispatch queue at creation time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var label: String { get }
```

## See Also

### Managing Queue Attributes

var qos: DispatchQoS

The quality-of-service level assgined to the queue.

func setTarget(queue: dispatch_queue_t?)

Specifies the dispatch queue on which to perform work associated with the current object.


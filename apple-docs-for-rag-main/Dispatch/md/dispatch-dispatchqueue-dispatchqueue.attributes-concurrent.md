

- Dispatch
- DispatchQueue
- DispatchQueue.Attributes
-  concurrent 

Type Property

# concurrent

The queue schedules tasks concurrently.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let concurrent: DispatchQueue.Attributes
```

## Discussion

If this attribute is not present, the queue schedules tasks serially in first-in, first-out (FIFO) order.

## See Also

### Attributes

static let initiallyInactive: DispatchQueue.Attributes

The newly created queue is inactive.


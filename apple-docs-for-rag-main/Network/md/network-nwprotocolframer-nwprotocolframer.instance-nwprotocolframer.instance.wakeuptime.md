

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  NWProtocolFramer.Instance.WakeupTime 

Enumeration

# NWProtocolFramer.Instance.WakeupTime

Times at which to schedule a protocol wakeup.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum WakeupTime
```

## Topics

### Time Values

case milliseconds(UInt64)

A specific number of milliseconds from now.

case forever

A sentinel value to indicate that no wakeup should be delivered.

## See Also

### Handling Asynchronous Events

func async(execute: () -> Void)

Requests that a block be executed on the connection’s internal scheduling context.

func scheduleWakeup(wakeupTime: NWProtocolFramer.Instance.WakeupTime)

Requests that wakeup(framer:) be called on your protocol at a specific time in the future.




- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  scheduleWakeup(wakeupTime:) 

Instance Method

# scheduleWakeup(wakeupTime:)

Requests that wakeup(framer:) be called on your protocol at a specific time in the future.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func scheduleWakeup(wakeupTime: NWProtocolFramer.Instance.WakeupTime)
```

## See Also

### Handling Asynchronous Events

func async(execute: () -> Void)

Requests that a block be executed on the connection’s internal scheduling context.

enum WakeupTime

Times at which to schedule a protocol wakeup.


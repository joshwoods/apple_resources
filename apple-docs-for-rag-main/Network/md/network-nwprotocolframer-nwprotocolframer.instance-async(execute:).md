

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  async(execute:) 

Instance Method

# async(execute:)

Requests that a block be executed on the connection’s internal scheduling context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func async(execute: @escaping () -> Void)
```

## Discussion

You should call this if you need to call any framer functions but are in another scheduling context.

## See Also

### Handling Asynchronous Events

func scheduleWakeup(wakeupTime: NWProtocolFramer.Instance.WakeupTime)

Requests that wakeup(framer:) be called on your protocol at a specific time in the future.

enum WakeupTime

Times at which to schedule a protocol wakeup.


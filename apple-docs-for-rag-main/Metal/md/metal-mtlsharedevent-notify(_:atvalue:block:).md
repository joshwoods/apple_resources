

- Metal
- MTLSharedEvent
-  notify(\_:atValue:block:) 

Instance Method

# notify(\_:atValue:block:)

Schedules a notification handler to be called after the shareable event’s signal value equals or exceeds a given value.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func notify(
    _ listener: MTLSharedEventListener,
    atValue value: UInt64,
    block: @escaping MTLSharedEventNotificationBlock
)
```

**Required**

## Parameters 

`listener`  

The listener object used to dispatch the notification.

`value`  

The minimum value that needs to be signaled before the notification handler is called.

`block`  

The notification handler to call.

## Mentioned in 

Synchronizing Events Between a GPU and the CPU

## See Also

### Synchronizing a Shareable Event

var signaledValue: UInt64

The current signal value for the shareable event.

**Required**


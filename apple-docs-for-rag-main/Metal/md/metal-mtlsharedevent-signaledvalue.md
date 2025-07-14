

- Metal
- MTLSharedEvent
-  signaledValue 

Instance Property

# signaledValue

The current signal value for the shareable event.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var signaledValue: UInt64 { get set }
```

**Required**

## Mentioned in 

Synchronizing Events Between a GPU and the CPU

## Discussion

When you set the value of a shared event, its value is changed only if you provide a larger value than the value currently stored in the event. Setting this property signals the event. Commands waiting on the event are allowed to run if the new value is equal to or greater than the value for which they are waiting. Similarly, setting the event’s value triggers notifications if the value is equal to or greater than the value for which they are waiting.

## See Also

### Synchronizing a Shareable Event

func notify(MTLSharedEventListener, atValue: UInt64, block: MTLSharedEventNotificationBlock)

Schedules a notification handler to be called after the shareable event’s signal value equals or exceeds a given value.

**Required**


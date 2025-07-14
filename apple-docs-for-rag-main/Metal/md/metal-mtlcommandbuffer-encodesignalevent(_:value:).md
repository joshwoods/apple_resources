

- Metal
- MTLCommandBuffer
-  encodeSignalEvent(\_:value:) 

Instance Method

# encodeSignalEvent(\_:value:)

Encodes a command that updates an event’s value, which can clear the GPU to run passes from other command buffers waiting for the event.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func encodeSignalEvent(
    _ event: any MTLEvent,
    value: UInt64
)
```

**Required**

## Parameters 

`event`  

An MTLEvent instance the GPU driver signals between passes as it runs the command buffer.

If `event` is an MTLSharedEvent instance, the update:

- Signals any command buffers waiting for the shared event, including those on other GPU devices

- Invokes any notification handlers waiting for the shared event (see notify(_:atValue:block:))

Otherwise, the method can signal only command buffers from the same GPU device.

`value`  

A value that’s greater than or equal to the event’s current value; otherwise, the command has no effect.

## Mentioned in 

About Synchronization Events

## Discussion

The method can unblock one or more command buffers that are waiting for `event`, including those in other command queues (see encodeWaitForEvent(_:value:)).

A command buffer can signal an event only between passes, not within a pass. If a command buffer has an active encoder, finish using the encoder, call its endEncoding() method, and then call this method before creating another encoder.

When the GPU device reaches the signal command that this method encodes, Metal updates the event after the GPU finishes the buffer’s prior commands. Updating the event’s value can signal any command buffer that’s waiting for a value equal to or less than the `value` parameter.

## See Also

### Synchronizing Passes with Events

func encodeWaitForEvent(any MTLEvent, value: UInt64)

Encodes a command into the command buffer that pauses the GPU from running the buffer’s subsequent passes until the event equals or exceeds a value.

**Required**


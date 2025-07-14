

- Metal
- MTLIOCommandBuffer
-  waitForEvent(\_:value:) 

Instance Method

# waitForEvent(\_:value:)

Encodes a command that pauses the command buffer’s execution until another part of your app signals a shared event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func waitForEvent(
    _ event: any MTLSharedEvent,
    value: UInt64
)
```

**Required**

## Parameters 

`event`  

A shared event instance the method waits for.

`value`  

A value the method compares to the event’s value. The method returns when the event’s value is greater than or equal to `value`.

## See Also

### Synchronizing a Command Buffer

func signalEvent(any MTLSharedEvent, value: UInt64)

Encodes a command that signals a shared event to other parts of your app.

**Required**




- Metal
- MTLIOCommandBuffer
-  signalEvent(\_:value:) 

Instance Method

# signalEvent(\_:value:)

Encodes a command that signals a shared event to other parts of your app.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func signalEvent(
    _ event: any MTLSharedEvent,
    value: UInt64
)
```

**Required**

## Parameters 

`event`  

A shared event instance the method waits for.

`value`  

A value the command uses to signal for the event to other parts of your app.

## See Also

### Synchronizing a Command Buffer

func waitForEvent(any MTLSharedEvent, value: UInt64)

Encodes a command that pauses the command buffer’s execution until another part of your app signals a shared event.

**Required**


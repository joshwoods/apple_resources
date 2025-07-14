

- Core Media
-  CMBufferQueueSetValidationCallback(\_:callback:refcon:) 

Function

# CMBufferQueueSetValidationCallback(\_:callback:refcon:)

A validation callback for the queue to call before enqueuing buffers.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueSetValidationCallback(
    _ queue: CMBufferQueue,
    callback: CMBufferValidationCallback,
    refcon: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`queue`  

`CMBufferQueue` that will use the validation callback.

`callback`  

Callback that will validate each buffer enqueued.

`refcon`  

Context refcon for validation callback.

## Return Value

A result code. See `Result Codes`.

## See Also

### Validating a Queue

func CMBufferQueueSetValidationHandler(CMBufferQueue, CMBufferValidationHandler) -> OSStatus

A validation handler for the queue to call before enqueuing buffers.

typealias CMBufferValidationHandler

A type alias for a handler that tests whether a buffer is in a valid state to add to a queue.

typealias CMBufferValidationCallback

A type alias for a callback that tests whether a buffer is in a valid state to add to a queue.


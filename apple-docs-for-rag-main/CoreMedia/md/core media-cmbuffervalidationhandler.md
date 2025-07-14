

- Core Media
-  CMBufferValidationHandler 

Type Alias

# CMBufferValidationHandler

A type alias for a handler that tests whether a buffer is in a valid state to add to a queue.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.14.4+tvOS 12.2+visionOS 1.0+watchOS 6.0+

``` source
typealias CMBufferValidationHandler = (CMBufferQueue, CMBuffer) -> OSStatus
```

## See Also

### Validating a Queue

func CMBufferQueueSetValidationHandler(CMBufferQueue, CMBufferValidationHandler) -> OSStatus

A validation handler for the queue to call before enqueuing buffers.

func CMBufferQueueSetValidationCallback(CMBufferQueue, callback: CMBufferValidationCallback, refcon: UnsafeMutableRawPointer?) -> OSStatus

A validation callback for the queue to call before enqueuing buffers.

typealias CMBufferValidationCallback

A type alias for a callback that tests whether a buffer is in a valid state to add to a queue.


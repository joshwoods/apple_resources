

- Matter
-  MTRAsyncCallbackQueueWorkItem Deprecated

Class

# MTRAsyncCallbackQueueWorkItem

iOS 16.1–17.2DeprecatediPadOS 16.1–17.2DeprecatedMac Catalyst 16.1–17.2DeprecatedmacOS 13.0–14.2DeprecatedtvOS 16.1–17.2DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–10.2Deprecated

``` source
class MTRAsyncCallbackQueueWorkItem
```

Deprecated

This class was not intended to be part of the public Matter API

## Topics

### Initializers

init(queue: dispatch_queue_t)

### Instance Properties

var cancelHandler: () -> Void

var readyHandler: MTRAsyncCallbackReadyHandler

### Instance Methods

func endWork()

func retryWork()

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol




- Core Media
- CMBufferQueue
-  CMBufferQueue.Handlers 

Structure

# CMBufferQueue.Handlers

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Handlers
```

## Topics

### Initializers

init(withHandlers: (inout CMBufferQueue.Handlers.Builder) -> Void)

### Instance Properties

let compare: CMBufferCompareHandler?

let dataBecameReadyNotification: String?

let getDecodeTimeStamp: CMBufferGetTimeHandler?

let getDuration: CMBufferGetTimeHandler

let getPresentationTimeStamp: CMBufferGetTimeHandler?

let getSize: CMBufferGetSizeHandler?

let isDataReady: CMBufferGetBooleanHandler?

### Type Properties

static let outputPTSSortedSampleBuffers: CMBufferQueue.Handlers

static let unsortedSampleBuffers: CMBufferQueue.Handlers

### Instance Methods

func withHandlers((inout CMBufferQueue.Handlers.Builder) -> Void) -> CMBufferQueue.Handlers

### Structures

struct Builder

## Relationships

### Conforms To

- Sendable

## See Also

### Data Types

struct Buffers

struct Error


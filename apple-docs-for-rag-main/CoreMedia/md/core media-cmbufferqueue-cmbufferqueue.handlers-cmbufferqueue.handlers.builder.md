

- Core Media
- CMBufferQueue
- CMBufferQueue.Handlers
-  CMBufferQueue.Handlers.Builder 

Structure

# CMBufferQueue.Handlers.Builder

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Builder
```

## Topics

### Instance Properties

var dataBecameReadyNotification: String?

### Instance Methods

func compare(CMBufferCompareHandler)

func getDecodeTimeStamp(CMBufferGetTimeHandler)

func getDuration(CMBufferGetTimeHandler)

func getPresentationTimeStamp(CMBufferGetTimeHandler)

func getSize(CMBufferGetSizeHandler)

func isDataReady(CMBufferGetBooleanHandler)

## Relationships

### Conforms To

- Sendable


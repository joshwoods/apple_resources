

- AVFoundation
- AVPlayerLooper
-  AVPlayerLooper.ItemOrdering 

Enumeration

# AVPlayerLooper.ItemOrdering

Constants that define the ordering of items in a player looper.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum ItemOrdering
```

## Topics

### Ordering

case loopingItemsPrecedeExistingItems

Indicates to insert replica items before any existing items in the specified player’s queue.

case loopingItemsFollowExistingItems

Indicates to insert replica items after any existing items in the specified player’s queue.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable


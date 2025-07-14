

- File Provider
-  NSFileProviderContentPolicy 

Enumeration

# NSFileProviderContentPolicy

iOS 16.0+iPadOS 16.0+macOS 13.0+visionOS 1.0+

``` source
enum NSFileProviderContentPolicy
```

## Topics

### Policies

case downloadEagerlyAndKeepDownloaded

case downloadLazily

case downloadLazilyAndEvictOnRemoteUpdate

case inherited

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Content

var childItemCount: NSNumber?

The number of items contained by this item.

var documentSize: NSNumber?

The document’s size, in bytes.

var contentPolicy: NSFileProviderContentPolicy


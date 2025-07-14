

- AVFoundation
-  AVAssetDownloadedAssetEvictionPriority 

Structure

# AVAssetDownloadedAssetEvictionPriority

Constants that define eviction priorities for a storage management policy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
struct AVAssetDownloadedAssetEvictionPriority
```

## Topics

### Eviction Priorities

static let `default`: AVAssetDownloadedAssetEvictionPriority

The default eviction priority.

static let important: AVAssetDownloadedAssetEvictionPriority

An eviction priority that indicates that this asset is important and the system should evict lower-priority assets first.

### Initializers

init(rawValue: String)

Creates an eviction priority with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Storage

var expirationDate: Date

The expiration date for an asset.

var priority: AVAssetDownloadedAssetEvictionPriority

The eviction priority for a downloaded asset.


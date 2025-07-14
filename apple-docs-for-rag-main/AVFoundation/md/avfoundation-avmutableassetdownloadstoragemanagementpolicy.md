

- AVFoundation
-  AVMutableAssetDownloadStorageManagementPolicy 

Class

# AVMutableAssetDownloadStorageManagementPolicy

A mutable object that you use to create a new storage management policy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class AVMutableAssetDownloadStorageManagementPolicy
```

## Topics

### Managing Storage

var expirationDate: Date

The expiration date for an asset.

var priority: AVAssetDownloadedAssetEvictionPriority

The eviction priority for a downloaded asset.

struct AVAssetDownloadedAssetEvictionPriority

Constants that define eviction priorities for a storage management policy.

## Relationships

### Inherits From

- AVAssetDownloadStorageManagementPolicy

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Offline storage management

class AVAssetDownloadStorageManager

An object that manages policies to automatically purge downloaded assets.

class AVAssetDownloadStorageManagementPolicy

An object that defines a policy to automatically manage the storage of downloaded assets.


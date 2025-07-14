

- AVFoundation
-  AVAssetDownloadStorageManagementPolicy 

Class

# AVAssetDownloadStorageManagementPolicy

An object that defines a policy to automatically manage the storage of downloaded assets.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class AVAssetDownloadStorageManagementPolicy
```

## Topics

### Inspecting a Policy

var expirationDate: Date

The expiration date for an asset.

var priority: AVAssetDownloadedAssetEvictionPriority

The eviction priority for an asset.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableAssetDownloadStorageManagementPolicy

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

class AVMutableAssetDownloadStorageManagementPolicy

A mutable object that you use to create a new storage management policy.


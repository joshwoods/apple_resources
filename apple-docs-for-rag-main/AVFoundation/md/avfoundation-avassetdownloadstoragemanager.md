

- AVFoundation
-  AVAssetDownloadStorageManager 

Class

# AVAssetDownloadStorageManager

An object that manages policies to automatically purge downloaded assets.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class AVAssetDownloadStorageManager
```

## Topics

### Accessing the Shared Manager

class func shared() -> AVAssetDownloadStorageManager

Returns the shared storage manager instance.

### Setting the Storage Policy

func storageManagementPolicy(for: URL) -> AVAssetDownloadStorageManagementPolicy?

Returns the storage management policy for a downloaded asset.

func setStorageManagementPolicy(AVAssetDownloadStorageManagementPolicy, for: URL)

Sets a storage policy for the downloaded asset.

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
- Sendable

## See Also

### Offline storage management

class AVAssetDownloadStorageManagementPolicy

An object that defines a policy to automatically manage the storage of downloaded assets.

class AVMutableAssetDownloadStorageManagementPolicy

A mutable object that you use to create a new storage management policy.


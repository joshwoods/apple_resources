

- AVFoundation
- AVAssetDownloadStorageManager
-  storageManagementPolicy(for:) 

Instance Method

# storageManagementPolicy(for:)

Returns the storage management policy for a downloaded asset.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func storageManagementPolicy(for downloadStorageURL: URL) -> AVAssetDownloadStorageManagementPolicy?
```

## Parameters 

`downloadStorageURL`  

The location of the downloaded asset.

## Return Value

The storage management policy for the asset, or `nil` if one isn’t set.

## See Also

### Setting the Storage Policy

func setStorageManagementPolicy(AVAssetDownloadStorageManagementPolicy, for: URL)

Sets a storage policy for the downloaded asset.




- AVFoundation
- AVAssetDownloadStorageManager
-  setStorageManagementPolicy(\_:for:) 

Instance Method

# setStorageManagementPolicy(\_:for:)

Sets a storage policy for the downloaded asset.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func setStorageManagementPolicy(
    _ storageManagementPolicy: AVAssetDownloadStorageManagementPolicy,
    for downloadStorageURL: URL
)
```

## Parameters 

`storageManagementPolicy`  

The policy to set for the downloaded asset.

`downloadStorageURL`  

The location of the downloaded asset.

## See Also

### Setting the Storage Policy

func storageManagementPolicy(for: URL) -> AVAssetDownloadStorageManagementPolicy?

Returns the storage management policy for a downloaded asset.


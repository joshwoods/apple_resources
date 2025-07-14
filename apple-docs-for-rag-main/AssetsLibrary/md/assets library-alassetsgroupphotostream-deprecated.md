

- Assets Library
-  ALAssetsGroupPhotoStream Deprecated

Global Variable

# ALAssetsGroupPhotoStream

The PhotoStream album.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var ALAssetsGroupPhotoStream: UInt32 { get }
```

Deprecated

Use PHAssetCollectionType and PHAssetCollectionSubtype in the Photos framework instead

## Discussion

In iOS 6.0 and later, this also includes Shared Streams.

## See Also

### Constants

var ALAssetsGroupLibrary: UInt32

The Library group that includes all assets that are synced from iTunes.

Deprecated

var ALAssetsGroupAlbum: UInt32

All the albums created on the device or synced from iTunes, not including Photo Stream or Shared Streams

Deprecated

var ALAssetsGroupEvent: UInt32

All events, including those created during Camera Connection Kit import.

Deprecated

var ALAssetsGroupFaces: UInt32

All the faces albums synced from iTunes.

Deprecated

var ALAssetsGroupSavedPhotos: UInt32

All the photos in the Camera Roll.

Deprecated

var ALAssetsGroupAll: UInt32

The same as ORing together all the group types except for ALAssetsGroupLibrary.

Deprecated


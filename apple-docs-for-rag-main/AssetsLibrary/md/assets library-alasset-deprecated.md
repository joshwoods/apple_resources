

- Assets Library
-  ALAsset Deprecated

Class

# ALAsset

An `ALAsset` object represents a photo or a video managed by the Photo application.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class ALAsset
```

Deprecated

Use PHAsset from the Photos framework instead

## Overview

Important

The Assets Library framework is deprecated as of iOS 9.0. Instead, use the Photos framework instead, which in iOS 8.0 and later provides more features and better performance for working with a user’s photo library. For more information, see `Photos`.

In the Photos framework, the PHAsset class provides functionality for fetching and working with photo and video assets.

Assets can have multiple representations, for example a photo which was captured in RAW and JPG. Different representations of the same asset may have different dimensions.

## Topics

### Asset Properties

func value(forProperty: String!) -> Any!

Returns the value for a given property.

var isEditable: Bool

Indicates whether the asset is editable.

var original: ALAsset!

The original version of the asset.

### Accessing Representations

func defaultRepresentation() -> ALAssetRepresentation!

Returns an asset representation object for the default representation.

func representation(forUTI: String!) -> ALAssetRepresentation!

Returns an asset representation object for a given representation UTI.

func thumbnail() -> Unmanaged&lt;CGImage>!

Returns a thumbnail representation of the asset.

func aspectRatioThumbnail() -> Unmanaged&lt;CGImage>!

Returns an aspect ratio thumbnail of the asset.

### Setting New Image and Video Data

func setImageData(Data!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Replaces the image data in the receiver with given image data

func setVideoAtPath(URL!, completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!)

Replaces the video data in receiver with the video at a given URL.

### Saving to the Saved Photos Album

func writeModifiedImageData(toSavedPhotosAlbum: Data!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Saves image data to the Saved Photos album.

func writeModifiedVideoAtPath(toSavedPhotosAlbum: URL!, completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!)

Saves the video at a specified path to the Saved Photos album.

### Constants

Property Keys

Constants for the keys for the properties you can get from an asset.

Invalid Property Value

A constant to indicate that a property accessed by value(forProperty:) is invalid.

Asset Types

Constants that specify the type of an asset.

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

## See Also

### Classes

class ALAssetRepresentation

An `ALAssetRepresentation` object encapsulates one of the representations of a given ALAsset object.

Deprecated

class ALAssetsFilter

`ALAssetsFilter` encapsulates filtering criteria to be used when retrieving assets from a group.

Deprecated

class ALAssetsGroup

An `ALAssetsGroup` object represents an ordered set of the assets managed by the Photos application. The order of the elements is the same as the user sees in the Photos application. An asset can belong to multiple assets groups.

Deprecated

class ALAssetsLibrary

An instance of `ALAssetsLibrary` provides access to the videos and photos that are under the control of the Photos application.

Deprecated


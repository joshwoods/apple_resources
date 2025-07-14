

- Assets Library
-  ALAssetRepresentation Deprecated

Class

# ALAssetRepresentation

An `ALAssetRepresentation` object encapsulates one of the representations of a given ALAsset object.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class ALAssetRepresentation
```

Deprecated

Use PHImageRequestOptions with the PHImageManager from the Photos framework instead

## Overview

Important

The Assets Library framework is deprecated as of iOS 9.0. Instead, use the Photos framework instead, which in iOS 8.0 and later provides more features and better performance for working with a user’s photo library. For more information, see `Photos`.

In the Photos framework, the PHAsset and PHImageManager classes provide functionality for fetching an asset’s image or video data.

A given asset in the library may have more than one representation. For example, if a camera provides RAW and JPEG versions of an image, the resulting asset will have two representations—one for the RAW file and one for the JPEG file.

## Topics

### Getting Image Representations

func cgImage(options: [AnyHashable : Any]!) -> Unmanaged&lt;CGImage>!

Returns a full resolution CGImage of the representation.

func fullResolutionImage() -> Unmanaged&lt;CGImage>!

Returns a CGImage representation of the asset.

func fullScreenImage() -> Unmanaged&lt;CGImage>!

Returns a CGImage of the representation that is appropriate for displaying full screen.

### Getting Image Attributes

func orientation() -> ALAssetOrientation

Returns the representation’s orientation.

func scale() -> Float

Returns the representation’s scale.

func dimensions() -> CGSize

Returns the representation’s dimensions.

func filename() -> String!

Returns a string representing the filename of the representation on disk.

### Getting Raw Data

func size() -> Int64

Returns the size in bytes of the file for the representation.

func getBytes(UnsafeMutablePointer&lt;UInt8>!, fromOffset: Int64, length: Int, error: NSErrorPointer) -> Int

Copies a specified range of bytes into a given buffer.

### Getting Metadata

func uti() -> String!

Returns the representation’s UTI.

func metadata() -> [AnyHashable : Any]!

Returns a dictionary of dictionaries of metadata for the representation.

### Getting an URL

func url() -> URL!

Returns a persistent URL uniquely identifying the representation.

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

class ALAsset

An `ALAsset` object represents a photo or a video managed by the Photo application.

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


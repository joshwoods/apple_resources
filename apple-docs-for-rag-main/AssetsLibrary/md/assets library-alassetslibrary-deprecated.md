

- Assets Library
-  ALAssetsLibrary Deprecated

Class

# ALAssetsLibrary

An instance of `ALAssetsLibrary` provides access to the videos and photos that are under the control of the Photos application.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class ALAssetsLibrary
```

Deprecated

Use PHPhotoLibrary from the Photos framework instead

## Overview

Important

The Assets Library framework is deprecated as of iOS 9.0. Instead, use the Photos framework instead, which in iOS 8.0 and later provides more features and better performance for working with a user’s photo library. For more information, see `Photos`.

In the Photos framework, the PHPhotoLibrary class manages access to and changes in the photo library, and class methods on the PHAsset and PHCollection classes and related classes provide functionality for finding photo and video assets.

The library includes those that are in the Saved Photos album, those coming from iTunes, and those that were directly imported into the device. You use it to retrieve the list of all asset groups and to save images and videos into the Saved Photos album.

You create an instance of `ALAssetsLibrary` using `alloc` and `init`:

```
```

The lifetimes of objects you get back from a library instance are tied to the lifetime of the library instance.

Many of the methods declared by `ALAssetsLibrary` take blocks for failure and success as arguments. These methods are all asynchronous because the user may need to be asked to grant access to the data.

## Topics

### Accessing Assets

class func authorizationStatus() -> ALAuthorizationStatus

Returns photo data authorization status for this application.

### Managing Notifications

class func disableSharedPhotoStreamsSupport()

Disables shared photo streams notifications and asset retrieval.

### Finding Assets

func asset(for: URL!, resultBlock: ALAssetsLibraryAssetForURLResultBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)

Invokes a given block passing as a parameter an asset identified by a specified file URL.

### Enumerating Assets

func enumerateGroups(withTypes: ALAssetsGroupType, using: ALAssetsLibraryGroupsEnumerationResultsBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)

Invokes a given block passing as a parameter each of the asset groups that match the given asset group type.

func enumerateGroupsWithTypes(UInt32, usingBlock: ALAssetsLibraryGroupsEnumerationResultsBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)

### Saving Assets

func writeVideoAtPath(toSavedPhotosAlbum: URL!, completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!)

Saves a video identified by a given URL to the Saved Photos album.

func videoAtPathIs(compatibleWithSavedPhotosAlbum: URL!) -> Bool

Returns a Boolean value that indicates whether a video identified by a given URL is compatible with the Saved Photos album.

func writeImage(toSavedPhotosAlbum: CGImage!, orientation: ALAssetOrientation, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Saves a given image to the Saved Photos album.

func writeImageData(toSavedPhotosAlbum: Data!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Writes given image data and metadata to the Photos Album.

func writeImage(toSavedPhotosAlbum: CGImage!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Writes a given image and metadata to the Photos Album.

### Managing Asset Groups

func addAssetsGroupAlbum(withName: String!, resultBlock: ALAssetsLibraryGroupResultBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)

Adds a new assets group to the library.

func group(for: URL!, resultBlock: ALAssetsLibraryGroupResultBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)

Returns an assets group in the result block for a URL previously retrieved from an `ALAssetsGroup` object.

### Constants

typealias ALAssetsGroupType

A bitfield to identify types of asset.

Types of Asset

Constants to identify types of asset.

enum ALAssetOrientation

Constants to indicate the orientation of an asset.

typealias ALAssetsLibraryGroupsEnumerationResultsBlock

Signature for the block executed when a match is found during enumeration using enumerateGroups(withTypes:using:failureBlock:).

typealias ALAssetsLibraryAssetForURLResultBlock

Signature for the block executed if the user has granted access to the caller to access the data managed by the framework in asset(for:resultBlock:failureBlock:).

typealias ALAssetsLibraryWriteImageCompletionBlock

Signature for the block executed when writeImage(toSavedPhotosAlbum:orientation:completionBlock:) completes.

typealias ALAssetsLibraryWriteVideoCompletionBlock

Signature for the block executed when writeVideoAtPath(toSavedPhotosAlbum:completionBlock:) completes.

typealias ALAssetsLibraryAccessFailureBlock

Signature for the block executed if the user does not grant access to the caller to access the data managed by the framework.

typealias ALAssetsLibraryGroupResultBlock

Signature for the block executed if the user grants access to the caller to access the data managed by the framework..

enum ALAuthorizationStatus

Constants to indicate authorization status.

Notification Keys

Keys used to get values from the user information dictionary of the ALAssetsLibraryChangedNotification notification.

Error Domain

Constant for the AssetsLibrary domain.

Error Codes

AssetsLibrary-related error codes

### Notifications

static let ALAssetsLibraryChanged: NSNotification.Name

Sent when the contents of the assets library have changed from under the app that is using the data.

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

class ALAssetRepresentation

An `ALAssetRepresentation` object encapsulates one of the representations of a given ALAsset object.

Deprecated

class ALAssetsFilter

`ALAssetsFilter` encapsulates filtering criteria to be used when retrieving assets from a group.

Deprecated

class ALAssetsGroup

An `ALAssetsGroup` object represents an ordered set of the assets managed by the Photos application. The order of the elements is the same as the user sees in the Photos application. An asset can belong to multiple assets groups.

Deprecated




- Assets Library
-  ALAssetsGroup Deprecated

Class

# ALAssetsGroup

An `ALAssetsGroup` object represents an ordered set of the assets managed by the Photos application. The order of the elements is the same as the user sees in the Photos application. An asset can belong to multiple assets groups.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class ALAssetsGroup
```

Deprecated

Use PHAssetCollection from the Photos framework instead

## Overview

Important

The Assets Library framework is deprecated as of iOS 9.0. Instead, use the Photos framework instead, which in iOS 8.0 and later provides more features and better performance for working with a user’s photo library. For more information, see `Photos`.

In the Photos framework, the PHCollection and PHCollectionList classes and their subclasses provide functionality for working with collections of assets.

Assets groups themselves are synced via iTunes, created to hold the user’s saved photos or created during camera import. You can indirectly modify the Saved Photos group by saving images or videos into it using the ALAssetsLibrary class.

## Topics

### Enumerating Assets

func enumerateAssets(ALAssetsGroupEnumerationResultsBlock!)

Invokes a given block using each of the assets in the group.

func enumerateAssets(options: NSEnumerationOptions, using: ALAssetsGroupEnumerationResultsBlock!)

Invokes a given block using each of the assets in the group.

func enumerateAssets(at: IndexSet!, options: NSEnumerationOptions, using: ALAssetsGroupEnumerationResultsBlock!)

Invokes a given block using each of the assets in the group at specified indexes.

### Adding Assets

func add(ALAsset!) -> Bool

Adds an existing asset to the receiver.

var isEditable: Bool

Indicates whether the application can edit the group.

### Filtering

func numberOfAssets() -> Int

Returns the number of assets in the group that match the current filter.

func setAssetsFilter(ALAssetsFilter!)

Sets the filter for the group.

### Accessing Properties

func value(forProperty: String!) -> Any!

Returns the group’s value for a given property.

func posterImage() -> Unmanaged&lt;CGImage>!

Returns the group’s poster image

### Constants

typealias ALAssetsGroupEnumerationResultsBlock

Signature for the block executed during enumeration of assets.

Group Property Names

Constants for the names of group properties, used by value(forProperty:).

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

class ALAssetsLibrary

An instance of `ALAssetsLibrary` provides access to the videos and photos that are under the control of the Photos application.

Deprecated


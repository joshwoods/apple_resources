

- Media Player
-  MPPlayableContentDataSource Deprecated

Protocol

# MPPlayableContentDataSource

The data source providing media metadata to external media players so they can build user interfaces displaying your app’s content.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
protocol MPPlayableContentDataSource : NSObjectProtocol
```

Deprecated

Use CarPlay framework

## Overview

To support external media players, create a class that conforms to the `MPPlayableContentDataSource` protocol. When your app launches, create an instance of this class and assign it to the shared dataSource property. This data source provides media metadata to external media players so that they can build user interfaces displaying your app’s content. It’s best to set this data source as early as possible in your app’s lifecycle, as iOS may start asking for content right away.

Important

This class is only used for CarPlay. Using it requires a special entitlement issued by Apple. Apps without the correct entitlement won’t appear on the CarPlay home screen. See http://www.apple.com/ios/carplay/ for more information.

## Topics

### Retrieving a media item

func contentItem(at: IndexPath) -> MPContentItem?

Retrieves the media item at the specified index.

**Required**

func contentItem(forIdentifier: String, completionHandler: (MPContentItem?, (any Error)?) -> Void)

Retrieves the content item associated with the provided identifier.

### Working with child nodes

func beginLoadingChildItems(at: IndexPath, completionHandler: ((any Error)?) -> Void)

Starts to load the children of the indicated index.

func childItemsDisplayPlaybackProgress(at: IndexPath) -> Bool

Returns a Boolean value indicating whether the provided content supports playback progress.

func numberOfChildItems(at: IndexPath) -> Int

Provides the number of child nodes for the indicated node.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Providing playable content

var dataSource: (any MPPlayableContentDataSource)?

The data source provided by the app.

Deprecated


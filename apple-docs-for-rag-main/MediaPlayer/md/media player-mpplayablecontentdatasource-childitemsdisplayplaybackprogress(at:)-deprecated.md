

- Media Player
- MPPlayableContentDataSource
-  childItemsDisplayPlaybackProgress(at:) Deprecated

Instance Method

# childItemsDisplayPlaybackProgress(at:)

Returns a Boolean value indicating whether the provided content supports playback progress.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func childItemsDisplayPlaybackProgress(at indexPath: IndexPath) -> Bool
```

Deprecated

Use CarPlay framework

## Parameters 

`indexPath`  

The index of the media item being queried.

## Return Value

Returns true if the indicated media item supports displaying playback progress.

## Discussion

If this method isn’t implemented, playback progress is not supported for any media item. If any media item does support displaying the playback progress, you must implement this method.

## See Also

### Working with child nodes

func beginLoadingChildItems(at: IndexPath, completionHandler: ((any Error)?) -> Void)

Starts to load the children of the indicated index.

Deprecated

func numberOfChildItems(at: IndexPath) -> Int

Provides the number of child nodes for the indicated node.

**Required**

Deprecated


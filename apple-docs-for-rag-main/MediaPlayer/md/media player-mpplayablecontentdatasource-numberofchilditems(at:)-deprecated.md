

- Media Player
- MPPlayableContentDataSource
-  numberOfChildItems(at:) Deprecated

Instance Method

# numberOfChildItems(at:)

Provides the number of child nodes for the indicated node.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func numberOfChildItems(at indexPath: IndexPath) -> Int
```

**Required**

Deprecated

Use CarPlay framework

## Parameters 

`indexPath`  

The index for the node to be queried.

## Return Value

An NSInteger value representing the number of child nodes associated with the indicated node.

## See Also

### Working with child nodes

func beginLoadingChildItems(at: IndexPath, completionHandler: ((any Error)?) -> Void)

Starts to load the children of the indicated index.

Deprecated

func childItemsDisplayPlaybackProgress(at: IndexPath) -> Bool

Returns a Boolean value indicating whether the provided content supports playback progress.

Deprecated


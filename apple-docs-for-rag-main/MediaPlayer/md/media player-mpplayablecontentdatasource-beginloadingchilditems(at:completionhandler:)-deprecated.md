

- Media Player
- MPPlayableContentDataSource
-  beginLoadingChildItems(at:completionHandler:) Deprecated

Instance Method

# beginLoadingChildItems(at:completionHandler:)

Starts to load the children of the indicated index.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func beginLoadingChildItems(
    at indexPath: IndexPath,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
optional func beginLoadingChildItems(at indexPath: IndexPath) async throws
```

Deprecated

Use CarPlay framework

## Parameters 

`indexPath`  

The index of the current item.

`completionHandler`  

A block to be called after all loading is completed.

The block receives the following parameter:

*error*  
Contains an error message if there was an error trying to load the children of the indicated item; otherwise, contains `nil`.

## Discussion

Call this method to start asynchronous batch loading of media items. The app can load content before the media player needs to display the next media items. When you use this method, the client app must call the completion handler after loading has finished.

## See Also

### Working with child nodes

func childItemsDisplayPlaybackProgress(at: IndexPath) -> Bool

Returns a Boolean value indicating whether the provided content supports playback progress.

Deprecated

func numberOfChildItems(at: IndexPath) -> Int

Provides the number of child nodes for the indicated node.

**Required**

Deprecated


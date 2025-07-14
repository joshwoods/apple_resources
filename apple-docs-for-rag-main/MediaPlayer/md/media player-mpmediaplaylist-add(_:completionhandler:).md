

- Media Player
- MPMediaPlaylist
-  add(\_:completionHandler:) 

Instance Method

# add(\_:completionHandler:)

Adds an array of media items to the end of the playlist.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
func add(
    _ mediaItems: [MPMediaItem],
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func add(_ mediaItems: [MPMediaItem]) async throws
```

## Parameters 

`mediaItems`  

The array of media items to add to the end of the playlist.

`completionHandler`  

A block that the system calls after it adds the media items to the playlist.

error  
If an error occurred, this parameter holds the error object that explains the error. Otherwise, the value of this parameter is nil.

## See Also

### Adding media items to a playlist

func addItem(withProductID: String, completionHandler: (((any Error)?) -> Void)?)

Adds the item associated with the product identifier to the end of the playlist.


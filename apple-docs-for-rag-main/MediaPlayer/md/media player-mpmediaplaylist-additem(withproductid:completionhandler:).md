

- Media Player
- MPMediaPlaylist
-  addItem(withProductID:completionHandler:) 

Instance Method

# addItem(withProductID:completionHandler:)

Adds the item associated with the product identifier to the end of the playlist.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
func addItem(
    withProductID productID: String,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func addItem(withProductID productID: String) async throws
```

## Parameters 

`productID`  

The product identifier for the item to add.

`completionHandler`  

A block that the system calls after it adds the item to the playlist.

error  
If an error occurred, this parameter holds the error object that explains the error. Otherwise, the value of this parameter is nil.

## Discussion

The method adds a single media item associated with the product identifier to the playlist.

## See Also

### Adding media items to a playlist

func add([MPMediaItem], completionHandler: (((any Error)?) -> Void)?)

Adds an array of media items to the end of the playlist.


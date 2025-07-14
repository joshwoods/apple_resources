

- Media Player
- MPMediaLibrary
-  addItem(withProductID:completionHandler:) 

Instance Method

# addItem(withProductID:completionHandler:)

Adds the designated item to the user’s music library.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
func addItem(
    withProductID productID: String,
    completionHandler: (([MPMediaEntity], (any Error)?) -> Void)? = nil
)
```

``` source
func addItem(withProductID productID: String) async throws -> [MPMediaEntity]
```

## Parameters 

`productID`  

The product identifier for the media item to add.

`completionHandler`  

A block that the system calls after it plays the media item.

entities  
An array containing the media items added to the user’s music library.

error  
If an error occurred, this parameter holds the error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

Use this method to add media items to a user’s music library. Use the Apple Music API Reference to search for content contained in the iTunes, App, Book, and Mac App stores.

Note

This method only works for 64-bit apps.


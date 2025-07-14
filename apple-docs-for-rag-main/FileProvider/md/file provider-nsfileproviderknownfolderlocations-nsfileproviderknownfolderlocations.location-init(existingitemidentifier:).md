

- File Provider
- NSFileProviderKnownFolderLocations
- NSFileProviderKnownFolderLocations.Location
-  init(existingItemIdentifier:) 

Initializer

# init(existingItemIdentifier:)

Initialize a location with the item identifier of a folder that already exists on the server.

macOS 15.0+

``` source
init(existingItemIdentifier: NSFileProviderItemIdentifier)
```

## Discussion

If the known folder already exists on the server, the provider can specify the exact identifier of the item that needs to be used to back the known folder.


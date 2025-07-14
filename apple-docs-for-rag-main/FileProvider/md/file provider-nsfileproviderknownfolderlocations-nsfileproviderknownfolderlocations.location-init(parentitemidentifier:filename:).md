

- File Provider
- NSFileProviderKnownFolderLocations
- NSFileProviderKnownFolderLocations.Location
-  init(parentItemIdentifier:filename:) 

Initializer

# init(parentItemIdentifier:filename:)

Initialize a location with the filename of the folder in a specified parent.

macOS 15.0+

``` source
init(
    parentItemIdentifier: NSFileProviderItemIdentifier,
    filename: String
)
```

## Discussion

When replicating a known folder the system will reuse a folder located at the specified filename within the parent if one exists, or create a new item at this location if none exists yet.


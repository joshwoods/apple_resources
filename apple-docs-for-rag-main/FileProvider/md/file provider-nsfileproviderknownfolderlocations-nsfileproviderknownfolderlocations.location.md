

- File Provider
- NSFileProviderKnownFolderLocations
-  NSFileProviderKnownFolderLocations.Location 

Class

# NSFileProviderKnownFolderLocations.Location

macOS 15.0+

``` source
class Location
```

## Topics

### Initializers

init(existingItemIdentifier: NSFileProviderItemIdentifier)

Initialize a location with the item identifier of a folder that already exists on the server.

init(parentItemIdentifier: NSFileProviderItemIdentifier, filename: String)

Initialize a location with the filename of the folder in a specified parent.

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

### Identifying known-folder locations

var desktopLocation: NSFileProviderKnownFolderLocations.Location?

var documentsLocation: NSFileProviderKnownFolderLocations.Location?


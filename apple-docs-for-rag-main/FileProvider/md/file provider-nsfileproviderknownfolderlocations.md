

- File Provider
-  NSFileProviderKnownFolderLocations 

Class

# NSFileProviderKnownFolderLocations

A class for working with known-folder locations.

macOS 15.0+

``` source
class NSFileProviderKnownFolderLocations
```

## Topics

### Identifying known-folder locations

var desktopLocation: NSFileProviderKnownFolderLocations.Location?

var documentsLocation: NSFileProviderKnownFolderLocations.Location?

class Location

### Configuring folder options

var shouldCreateBinaryCompatibilitySymlink: Bool

### Creating a known-folder locations object

init()

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

### Syncing Desktop and Documents folders

func claimKnownFolders(NSFileProviderKnownFolderLocations, localizedReason: String, completionHandler: ((any Error)?) -> Void)

Asks the domain to sync the specified known folders.

func releaseKnownFolders(NSFileProviderKnownFolders, localizedReason: String, completionHandler: ((any Error)?) -> Void)

Asks the system to stop replicating the specified known folders in the domain.

struct NSFileProviderKnownFolders

Constants that identify known folders.

protocol NSFileProviderKnownFolderSupporting

A protocol that defines the interface for sharing known-folder locations with the system.




- File Provider
-  NSFileProviderKnownFolderSupporting 

Protocol

# NSFileProviderKnownFolderSupporting

A protocol that defines the interface for sharing known-folder locations with the system.

macOS 15.0+

``` source
protocol NSFileProviderKnownFolderSupporting : NSObjectProtocol
```

## Topics

### Providing known-folder locations to the system

func getKnownFolderLocations(NSFileProviderKnownFolders, completionHandler: (NSFileProviderKnownFolderLocations?, (any Error)?) -> Void)

Requests suitable locations for known folders.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Syncing Desktop and Documents folders

func claimKnownFolders(NSFileProviderKnownFolderLocations, localizedReason: String, completionHandler: ((any Error)?) -> Void)

Asks the domain to sync the specified known folders.

func releaseKnownFolders(NSFileProviderKnownFolders, localizedReason: String, completionHandler: ((any Error)?) -> Void)

Asks the system to stop replicating the specified known folders in the domain.

struct NSFileProviderKnownFolders

Constants that identify known folders.

class NSFileProviderKnownFolderLocations

A class for working with known-folder locations.


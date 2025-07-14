

- File Provider
- NSFileProviderManager
-  releaseKnownFolders(\_:localizedReason:completionHandler:) 

Instance Method

# releaseKnownFolders(\_:localizedReason:completionHandler:)

Asks the system to stop replicating the specified known folders in the domain.

macOS 15.0+

``` source
func releaseKnownFolders(
    _ knownFolders: NSFileProviderKnownFolders,
    localizedReason: String,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func releaseKnownFolders(
    _ knownFolders: NSFileProviderKnownFolders,
    localizedReason: String
) async throws
```

## Discussion

Use this method to immediately disable replication of the specified known folders.

## See Also

### Syncing Desktop and Documents folders

func claimKnownFolders(NSFileProviderKnownFolderLocations, localizedReason: String, completionHandler: ((any Error)?) -> Void)

Asks the domain to sync the specified known folders.

struct NSFileProviderKnownFolders

Constants that identify known folders.

class NSFileProviderKnownFolderLocations

A class for working with known-folder locations.

protocol NSFileProviderKnownFolderSupporting

A protocol that defines the interface for sharing known-folder locations with the system.


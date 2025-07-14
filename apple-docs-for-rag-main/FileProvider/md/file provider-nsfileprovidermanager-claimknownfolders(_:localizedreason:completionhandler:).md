

- File Provider
- NSFileProviderManager
-  claimKnownFolders(\_:localizedReason:completionHandler:) 

Instance Method

# claimKnownFolders(\_:localizedReason:completionHandler:)

Asks the domain to sync the specified known folders.

macOS 15.0+

``` source
func claimKnownFolders(
    _ knownFolders: NSFileProviderKnownFolderLocations,
    localizedReason: String,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func claimKnownFolders(
    _ knownFolders: NSFileProviderKnownFolderLocations,
    localizedReason: String
) async throws
```

## Discussion

Use this method to claim a set of known folders according to the information in the `knownFolders` parameter. The system only enables sync for these folders in the domain if the set of locations is valid and if the user agrees.

## See Also

### Syncing Desktop and Documents folders

func releaseKnownFolders(NSFileProviderKnownFolders, localizedReason: String, completionHandler: ((any Error)?) -> Void)

Asks the system to stop replicating the specified known folders in the domain.

struct NSFileProviderKnownFolders

Constants that identify known folders.

class NSFileProviderKnownFolderLocations

A class for working with known-folder locations.

protocol NSFileProviderKnownFolderSupporting

A protocol that defines the interface for sharing known-folder locations with the system.




- File Provider
- NSFileProviderKnownFolderSupporting
-  getKnownFolderLocations(\_:completionHandler:) 

Instance Method

# getKnownFolderLocations(\_:completionHandler:)

Requests suitable locations for known folders.

macOS 15.0+

``` source
func getKnownFolderLocations(
    _ knownFolders: NSFileProviderKnownFolders,
    completionHandler: @escaping (NSFileProviderKnownFolderLocations?, (any Error)?) -> Void
)
```

``` source
func knownFolderLocations(_ knownFolders: NSFileProviderKnownFolders) async throws -> NSFileProviderKnownFolderLocations
```

**Required**


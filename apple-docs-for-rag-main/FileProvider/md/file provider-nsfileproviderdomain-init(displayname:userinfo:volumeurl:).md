

- File Provider
- NSFileProviderDomain
-  init(displayName:userInfo:volumeURL:) 

Initializer

# init(displayName:userInfo:volumeURL:)

Creates a new file provider domain with the specified URL and display name.

macOS 15.0+

``` source
init(
    displayName: String,
    userInfo: [AnyHashable : Any] = [:],
    volumeURL: URL?
)
```

## See Also

### Creating domains

init(identifier: NSFileProviderDomainIdentifier, displayName: String, pathRelativeToDocumentStorage: String)

Returns a newly instantiated domain.

init(identifier: NSFileProviderDomainIdentifier, displayName: String)

Creates a new file provider domain with the specified identifier and display name.

struct NSFileProviderDomainIdentifier

A unique identifier for a file provider’s domain.


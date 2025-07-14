

- File Provider
- NSFileProviderDomain
-  init(identifier:displayName:pathRelativeToDocumentStorage:) 

Initializer

# init(identifier:displayName:pathRelativeToDocumentStorage:)

Returns a newly instantiated domain.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
init(
    identifier: NSFileProviderDomainIdentifier,
    displayName: String,
    pathRelativeToDocumentStorage: String
)
```

## Parameters 

`identifier`  

A string that identifies the domain. The file provider extension can select any string to uniquely identify the domain, as long as it doesn’t contain the colon (:) or slash (/) symbols.

`displayName`  

The name for the domain that the system shows to the user.

`pathRelativeToDocumentStorage`  

A path relative to the file provider extension’s documentStorageURL that the system uses to store the domain’s content.

## See Also

### Creating domains

init(identifier: NSFileProviderDomainIdentifier, displayName: String)

Creates a new file provider domain with the specified identifier and display name.

struct NSFileProviderDomainIdentifier

A unique identifier for a file provider’s domain.

init(displayName: String, userInfo: [AnyHashable : Any], volumeURL: URL?)

Creates a new file provider domain with the specified URL and display name.


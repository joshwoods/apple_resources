

- File Provider
-  NSFileProviderDomainIdentifier 

Structure

# NSFileProviderDomainIdentifier

A unique identifier for a file provider’s domain.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
struct NSFileProviderDomainIdentifier
```

## Topics

### Initializers

init(String)

Returns a newly initialized domain identifier.

init(rawValue: String)

Returns a newly initialized domain identifier.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating domains

init(identifier: NSFileProviderDomainIdentifier, displayName: String, pathRelativeToDocumentStorage: String)

Returns a newly instantiated domain.

init(identifier: NSFileProviderDomainIdentifier, displayName: String)

Creates a new file provider domain with the specified identifier and display name.

init(displayName: String, userInfo: [AnyHashable : Any], volumeURL: URL?)

Creates a new file provider domain with the specified URL and display name.


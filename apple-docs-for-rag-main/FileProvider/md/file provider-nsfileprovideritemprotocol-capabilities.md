

- File Provider
- NSFileProviderItemProtocol
-  capabilities 

Instance Property

# capabilities

The item’s capabilities.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
optional var capabilities: NSFileProviderItemCapabilities { get }
```

## See Also

### Providing Required Properties

var itemIdentifier: NSFileProviderItemIdentifier

The item’s persistent identifier.

**Required**

var filename: String

The item’s filename.

**Required**

var typeIdentifier: String

The item’s Uniform Type Identifier (UTI).

Deprecated

var contentType: UTType

The item’s Uniform Type Identifier (UTI).


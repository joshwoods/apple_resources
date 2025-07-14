

- File Provider
- NSFileProviderItemProtocol
-  filename 

Instance Property

# filename

The item’s filename.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
var filename: String { get }
```

**Required**

## See Also

### Providing Required Properties

var itemIdentifier: NSFileProviderItemIdentifier

The item’s persistent identifier.

**Required**

var typeIdentifier: String

The item’s Uniform Type Identifier (UTI).

Deprecated

var contentType: UTType

The item’s Uniform Type Identifier (UTI).

var capabilities: NSFileProviderItemCapabilities

The item’s capabilities.


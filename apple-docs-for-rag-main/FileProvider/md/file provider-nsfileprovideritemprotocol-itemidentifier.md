

- File Provider
- NSFileProviderItemProtocol
-  itemIdentifier 

Instance Property

# itemIdentifier

The item’s persistent identifier.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
var itemIdentifier: NSFileProviderItemIdentifier { get }
```

**Required**

## Mentioned in 

Using push notifications to signal changes

Synchronizing the File Provider Extension

## See Also

### Providing Required Properties

var filename: String

The item’s filename.

**Required**

var typeIdentifier: String

The item’s Uniform Type Identifier (UTI).

Deprecated

var contentType: UTType

The item’s Uniform Type Identifier (UTI).

var capabilities: NSFileProviderItemCapabilities

The item’s capabilities.




- File Provider
- NSFileProviderItemProtocol
-  contentType 

Instance Property

# contentType

The item’s Uniform Type Identifier (UTI).

iOS 14.0+iPadOS 14.0+macOS 11.0+visionOS 1.0+

``` source
@NSCopying
optional var contentType: UTType { get }
```

## Discussion

Your extension must provide either the typeIdentifier or the contentType property. Where possible, use the contentType property. Use the typeIdentifier property only in iOS 13 or earlier.

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

var capabilities: NSFileProviderItemCapabilities

The item’s capabilities.


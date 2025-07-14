

- File Provider
- NSFileProviderItemProtocol
-  typeIdentifier Deprecated

Instance Property

# typeIdentifier

The item’s Uniform Type Identifier (UTI).

iOS 11.0–15.0DeprecatediPadOS 11.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional var typeIdentifier: String { get }
```

Deprecated

Use contentType instead.

## Discussion

Your extension must provide either the typeIdentifier or the contentType property. Use the typeIdentifier property only in iOS 13 or earlier.

## See Also

### Providing Required Properties

var itemIdentifier: NSFileProviderItemIdentifier

The item’s persistent identifier.

**Required**

var filename: String

The item’s filename.

**Required**

var contentType: UTType

The item’s Uniform Type Identifier (UTI).

var capabilities: NSFileProviderItemCapabilities

The item’s capabilities.


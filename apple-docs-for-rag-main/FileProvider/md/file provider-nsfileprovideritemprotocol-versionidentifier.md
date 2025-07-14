

- File Provider
- NSFileProviderItemProtocol
-  versionIdentifier 

Instance Property

# versionIdentifier

A data value used to determine when the item changes.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
optional var versionIdentifier: Data? { get }
```

## Discussion

This property contains a data object that can uniquely identify each version of the item; for example, the hash of a document’s contents.

Version identifiers are limited to 1000 bytes.

## See Also

### Tracking Versions

var itemVersion: NSFileProviderItemVersion

A version object that tracks changes to an item.

var isMostRecentVersionDownloaded: Bool

A Boolean value that indicates whether the item is the most recent version downloaded from the server.


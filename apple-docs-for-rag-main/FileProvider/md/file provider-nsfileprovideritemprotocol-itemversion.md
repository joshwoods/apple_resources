

- File Provider
- NSFileProviderItemProtocol
-  itemVersion 

Instance Property

# itemVersion

A version object that tracks changes to an item.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
optional var itemVersion: NSFileProviderItemVersion { get }
```

## Discussion

The version object lets you track changes to an item’s content and metadata separately. Updating the version also invalidates the thumbnail cache. For more information, see NSFileProviderItemVersion.

## See Also

### Tracking Versions

var versionIdentifier: Data?

A data value used to determine when the item changes.

var isMostRecentVersionDownloaded: Bool

A Boolean value that indicates whether the item is the most recent version downloaded from the server.


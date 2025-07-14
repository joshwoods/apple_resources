

- File Provider
- NSFileProviderItemVersion
-  contentVersion 

Instance Property

# contentVersion

An opaque object used to track versions of the item’s content.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
var contentVersion: Data { get }
```

## Discussion

If the system stores a local copy of an item’s content, it downloads a new copy when the contentVersion changes. The content version also invalidates the system’s thumbnail cache.

The system considers the file’s resource fork part of the file’s content. The version changes when either the data fork or the resource fork changes.

The version data object must be no longer than 128 bytes.

## See Also

### Accessing Version Data

class var beforeFirstSyncComponent: Data

A Boolean value indicating that this version predates the version returned by the file provider extension.

var metadataVersion: Data

An opaque object used to track versions of the item’s metadata.


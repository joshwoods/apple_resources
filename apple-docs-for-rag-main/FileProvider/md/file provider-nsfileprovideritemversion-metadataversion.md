

- File Provider
- NSFileProviderItemVersion
-  metadataVersion 

Instance Property

# metadataVersion

An opaque object used to track versions of the item’s metadata.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
var metadataVersion: Data { get }
```

## Discussion

When the metadataVersion changes, system updates the dataless representation of the item on disk, but it doesn’t attempt to download the content.

The version data object must be no longer than 128 bytes.

## See Also

### Accessing Version Data

class var beforeFirstSyncComponent: Data

A Boolean value indicating that this version predates the version returned by the file provider extension.

var contentVersion: Data

An opaque object used to track versions of the item’s content.


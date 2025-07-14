

- Foundation
- NSFileCoordinator
- NSFileCoordinator.ReadingOptions
-  resolvesSymbolicLink 

Type Property

# resolvesSymbolicLink

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var resolvesSymbolicLink: NSFileCoordinator.ReadingOptions { get }
```

## Discussion

Specify this constant if you want an item that might be a symbolic link to resolve to the file pointed to by that link (instead of to the link itself). When you use this option, the system provides the resolved URL to the accessor block in place of the original URL.

Note

This option cannot be used with the prepare(forReadingItemsAt:options:writingItemsAt:options:error:byAccessor:) method.

## See Also

### Constants

static var withoutChanges: NSFileCoordinator.ReadingOptions

static var immediatelyAvailableMetadataOnly: NSFileCoordinator.ReadingOptions

Specify this constant if you want to read an item’s metadata without triggering a download.

static var forUploading: NSFileCoordinator.ReadingOptions

Specify this content when reading an item for the purpose of uploading its contents.


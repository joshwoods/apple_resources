

- Foundation
- NSFileCoordinator
- NSFileCoordinator.ReadingOptions
-  init(rawValue:) 

Initializer

# init(rawValue:)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(rawValue: UInt)
```

## See Also

### Creating a Reading Option

static var withoutChanges: NSFileCoordinator.ReadingOptions

static var resolvesSymbolicLink: NSFileCoordinator.ReadingOptions

static var immediatelyAvailableMetadataOnly: NSFileCoordinator.ReadingOptions

Specify this constant if you want to read an item’s metadata without triggering a download.

static var forUploading: NSFileCoordinator.ReadingOptions

Specify this content when reading an item for the purpose of uploading its contents.


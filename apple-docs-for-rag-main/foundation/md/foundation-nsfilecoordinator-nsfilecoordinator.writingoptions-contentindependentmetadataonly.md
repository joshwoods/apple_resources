

- Foundation
- NSFileCoordinator
- NSFileCoordinator.WritingOptions
-  contentIndependentMetadataOnly 

Type Property

# contentIndependentMetadataOnly

Select this option when writing to change the file’s metadata only and not its contents.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var contentIndependentMetadataOnly: NSFileCoordinator.WritingOptions { get }
```

## Discussion

Any changes written to the item’s contents during this coordinated write may not be preserved or may fail. Changing metadata that is related to the item’s content is also not supported, and those changes may not be preserved. For example, changing the value of tagNamesKey is supported, but changing the value of contentModificationDateKey is not.

## See Also

### Constants

static var forDeleting: NSFileCoordinator.WritingOptions

static var forMoving: NSFileCoordinator.WritingOptions

static var forMerging: NSFileCoordinator.WritingOptions

static var forReplacing: NSFileCoordinator.WritingOptions


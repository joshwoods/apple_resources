

- Foundation
- NSFileCoordinator
- NSFileCoordinator.WritingOptions
-  forMerging 

Type Property

# forMerging

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var forMerging: NSFileCoordinator.WritingOptions { get }
```

## Discussion

When this constant is specified, the file coordinator calls the savePresentedItemChanges(completionHandler:) method of relevant file presenters to give them a chance to save their changes before your code makes its changes.

## See Also

### Constants

static var forDeleting: NSFileCoordinator.WritingOptions

static var forMoving: NSFileCoordinator.WritingOptions

static var forReplacing: NSFileCoordinator.WritingOptions

static var contentIndependentMetadataOnly: NSFileCoordinator.WritingOptions

Select this option when writing to change the file’s metadata only and not its contents.


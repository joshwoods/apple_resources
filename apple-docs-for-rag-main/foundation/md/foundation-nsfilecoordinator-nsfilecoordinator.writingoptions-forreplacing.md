

- Foundation
- NSFileCoordinator
- NSFileCoordinator.WritingOptions
-  forReplacing 

Type Property

# forReplacing

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var forReplacing: NSFileCoordinator.WritingOptions { get }
```

## Discussion

Specifies whether the act of writing to the file involves actually replacing the file with a different file (or directory). If the current file coordinator is waiting for another object to move or rename the file, this option treats the operation as the creation of a new file (instead of as the replacement of the old file); otherwise, this constant causes the same behavior as the forDeleting constant. Use this method when the moving or creating an item should replace any item currently stored at that location. To avoid a race condition, use it regardless of whether an item is actually in the way before the writing begins. Do not use this method when simply updating the contents of the existing file.

## See Also

### Constants

static var forDeleting: NSFileCoordinator.WritingOptions

static var forMoving: NSFileCoordinator.WritingOptions

static var forMerging: NSFileCoordinator.WritingOptions

static var contentIndependentMetadataOnly: NSFileCoordinator.WritingOptions

Select this option when writing to change the file’s metadata only and not its contents.


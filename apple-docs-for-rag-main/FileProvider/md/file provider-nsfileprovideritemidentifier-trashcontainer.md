

- File Provider
- NSFileProviderItemIdentifier
-  trashContainer 

Type Property

# trashContainer

The persistent identifier for the parent of all trashed items.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
static let trashContainer: NSFileProviderItemIdentifier
```

## Discussion

When the user moves an item to the trash, the system sets its parentItemIdentifier to trashContainer. Your extension must enumerate all trashed items on request.

## See Also

### Constants

static let rootContainer: NSFileProviderItemIdentifier

The persistent identifier for the root directory of the file provider’s shared file hierarchy.

static let workingSet: NSFileProviderItemIdentifier

The persistent identifier representing the working set of documents and directories.


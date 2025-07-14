

- FSKit
- FSVolume
- FSVolume.Operations
-  createLink(to:named:inDirectory:replyHandler:) 

Instance Method

# createLink(to:named:inDirectory:replyHandler:)

Creates a new hard link.

macOS 15.4+

``` source
func createLink(
    to item: FSItem,
    named name: FSFileName,
    inDirectory directory: FSItem,
    replyHandler reply: @escaping (FSFileName?, (any Error)?) -> Void
)
```

``` source
func createLink(
    to item: FSItem,
    named name: FSFileName,
    inDirectory directory: FSItem
) async throws -> FSFileName
```

**Required**

## Parameters 

`item`  

The existing item to which to link.

`name`  

The name for the new link.

`directory`  

The directory in which to create the link.

`reply`  

A block or closure to indicate success or failure. If creation succeeds, pass an FSFileName of the newly-created link and a `nil` error. If creation fails, pass the relevant error as the second parameter; FSKit ignores any FSFileName in this case. For an `async` Swift implementation, there’s no reply handler; simply return the FSFileName or throw an error.

## Discussion

If creating the link fails, complete the request with an error with a domain of NSPOSIXErrorDomain and the following error codes:

- `EEXIST` if there’s already an item named `name` in the directory.

- `EMLINK` if creating the link would exceed the maximum number of hard links supported on `item`.

- `ENOTSUP` if the file system doesn’t support creating hard links to the type of file system object that `item` represents.

## See Also

### Working with links

func createSymbolicLink(named: FSFileName, inDirectory: FSItem, attributes: FSItem.SetAttributesRequest, linkContents: FSFileName, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Creates a new symbolic link.

**Required**

func readSymbolicLink(FSItem, replyHandler: (FSFileName?, (any Error)?) -> Void)

Reads a symbolic link.

**Required**


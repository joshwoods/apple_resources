

- FSKit
- FSVolume
- FSVolume.Operations
-  createSymbolicLink(named:inDirectory:attributes:linkContents:replyHandler:) 

Instance Method

# createSymbolicLink(named:inDirectory:attributes:linkContents:replyHandler:)

Creates a new symbolic link.

macOS 15.4+

``` source
func createSymbolicLink(
    named name: FSFileName,
    inDirectory directory: FSItem,
    attributes newAttributes: FSItem.SetAttributesRequest,
    linkContents contents: FSFileName,
    replyHandler reply: @escaping (FSItem?, FSFileName?, (any Error)?) -> Void
)
```

``` source
func createSymbolicLink(
    named name: FSFileName,
    inDirectory directory: FSItem,
    attributes newAttributes: FSItem.SetAttributesRequest,
    linkContents contents: FSFileName
) async throws -> (FSItem, FSFileName)
```

**Required**

## Parameters 

`name`  

The new item’s name.

`directory`  

The directory in which to create the item.

`newAttributes`  

Attributes to apply to the new item.

`contents`  

The contents of the new symbolic link.

`reply`  

A block or closure to indicate success or failure. If creation succeeds, pass the newly-created FSItem and a `nil` error. If creation fails, pass the relevant error as the second parameter; FSKit ignores any FSItem in this case. For an `async` Swift implementation, there’s no reply handler; simply return the FSItem or throw an error.

## Discussion

If an item named `name` already exists in the directory indicated by `directory`, complete the request with an error with a domain of NSPOSIXErrorDomain and a code of `EEXIST`.

## See Also

### Working with links

func createLink(to: FSItem, named: FSFileName, inDirectory: FSItem, replyHandler: (FSFileName?, (any Error)?) -> Void)

Creates a new hard link.

**Required**

func readSymbolicLink(FSItem, replyHandler: (FSFileName?, (any Error)?) -> Void)

Reads a symbolic link.

**Required**


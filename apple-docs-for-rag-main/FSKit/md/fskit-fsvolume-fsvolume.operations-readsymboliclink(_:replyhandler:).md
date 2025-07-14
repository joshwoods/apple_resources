

- FSKit
- FSVolume
- FSVolume.Operations
-  readSymbolicLink(\_:replyHandler:) 

Instance Method

# readSymbolicLink(\_:replyHandler:)

Reads a symbolic link.

macOS 15.4+

``` source
func readSymbolicLink(
    _ item: FSItem,
    replyHandler reply: @escaping (FSFileName?, (any Error)?) -> Void
)
```

``` source
func readSymbolicLink(_ item: FSItem) async throws -> FSFileName
```

**Required**

## Parameters 

`item`  

The symbolic link to read from. FSKit guarantees this item is of type FSItem.ItemType.symlink.

`reply`  

A block or closure to indicate success or failure. If reading succeeds, pass the link’s contents as an FSFileName and a `nil` error. If reading fails, pass the relevant error as the second parameter; FSKit ignores any FSFileName in this case. For an `async` Swift implementation, there’s no reply handler; simply return the FSFileName or throw an error.

## See Also

### Working with links

func createLink(to: FSItem, named: FSFileName, inDirectory: FSItem, replyHandler: (FSFileName?, (any Error)?) -> Void)

Creates a new hard link.

**Required**

func createSymbolicLink(named: FSFileName, inDirectory: FSItem, attributes: FSItem.SetAttributesRequest, linkContents: FSFileName, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Creates a new symbolic link.

**Required**


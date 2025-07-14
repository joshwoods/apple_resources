

- FSKit
- FSVolume
- FSVolume.Operations
-  lookupItem(named:inDirectory:replyHandler:) 

Instance Method

# lookupItem(named:inDirectory:replyHandler:)

Looks up an item within a directory.

macOS 15.4+

``` source
func lookupItem(
    named name: FSFileName,
    inDirectory directory: FSItem,
    replyHandler reply: @escaping (FSItem?, FSFileName?, (any Error)?) -> Void
)
```

``` source
func lookupItem(
    named name: FSFileName,
    inDirectory directory: FSItem
) async throws -> (FSItem, FSFileName)
```

**Required**

## Parameters 

`name`  

The name of the item to look up.

`directory`  

The directory in which to look up the item.

`reply`  

A block or closure to indicate success or failure. If lookup succeeds, pass the found FSItem and its FSFileName (as saved within the file system), along with a `nil` error. If lookup fails, pass the relevant error as the third parameter; any FSItem or FSFileName are ignored in this case. For an `async` Swift implementation, there’s no reply handler; simply return the FSItem and FSFileName as a tuple or throw an error.

## Discussion

If no item matching `name` exists in the directory indicated by `directory`, complete the request with an error with a domain of NSPOSIXErrorDomain and a code of `ENOENT`.

Tip

The FSFileName sent back to the caller may differ from the `name` parameter. This flexibility allows your implementation to handle case-insensitive and case-sensitive file systems. It might also be the case that `name` uses a composed Unicode string, but the name maintained by the file system and provided to the caller is uncomposed Unicode.

## See Also

### Working with items

func createItem(named: FSFileName, type: FSItem.ItemType, inDirectory: FSItem, attributes: FSItem.SetAttributesRequest, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Creates a new file or directory item.

**Required**

class FSFileName

The name of a file, expressed as a data buffer.

enum ItemType

An enumeration of item types, such as file, directory, or symbolic link.

class SetAttributesRequest

A request to set attributes on an item.

func removeItem(FSItem, named: FSFileName, fromDirectory: FSItem, replyHandler: ((any Error)?) -> Void)

Removes an existing item from a given directory.

**Required**

func renameItem(FSItem, inDirectory: FSItem, named: FSFileName, to: FSFileName, inDirectory: FSItem, overItem: FSItem?, replyHandler: (FSFileName?, (any Error)?) -> Void)

Renames an item from one path in the file system to another.

**Required**

func reclaimItem(FSItem, replyHandler: ((any Error)?) -> Void)

Reclaims an item, releasing any resources allocated for the item.

**Required**


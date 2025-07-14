

- FSKit
- FSVolume
- FSVolume.Operations
-  createItem(named:type:inDirectory:attributes:replyHandler:) 

Instance Method

# createItem(named:type:inDirectory:attributes:replyHandler:)

Creates a new file or directory item.

macOS 15.4+

``` source
func createItem(
    named name: FSFileName,
    type: FSItem.ItemType,
    inDirectory directory: FSItem,
    attributes newAttributes: FSItem.SetAttributesRequest,
    replyHandler reply: @escaping (FSItem?, FSFileName?, (any Error)?) -> Void
)
```

``` source
func createItem(
    named name: FSFileName,
    type: FSItem.ItemType,
    inDirectory directory: FSItem,
    attributes newAttributes: FSItem.SetAttributesRequest
) async throws -> (FSItem, FSFileName)
```

**Required**

## Parameters 

`name`  

The new item’s name.

`type`  

The new item’s type. Valid values are FSItem.ItemType.file or FSItem.ItemType.directory.

`directory`  

The directory in which to create the item.

`newAttributes`  

Attributes to apply to the new item.

`reply`  

A block or closure to indicate success or failure. If creation succeeds, pass the newly-created FSItem and its FSFileName, along with a `nil` error. If creation fails, pass the relevant error as the third parameter; FSKit ignores any FSItem or FSFileName in this case. For an `async` Swift implementation, there’s no reply handler; simply return a tuple of the FSItem and its FSFileName or throw an error.

## Discussion

If an item named `name` already exists in the directory indicated by `directory`, complete the request with an error with a domain of NSPOSIXErrorDomain and a code of `EEXIST`.

## See Also

### Working with items

class FSFileName

The name of a file, expressed as a data buffer.

enum ItemType

An enumeration of item types, such as file, directory, or symbolic link.

class SetAttributesRequest

A request to set attributes on an item.

func lookupItem(named: FSFileName, inDirectory: FSItem, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Looks up an item within a directory.

**Required**

func removeItem(FSItem, named: FSFileName, fromDirectory: FSItem, replyHandler: ((any Error)?) -> Void)

Removes an existing item from a given directory.

**Required**

func renameItem(FSItem, inDirectory: FSItem, named: FSFileName, to: FSFileName, inDirectory: FSItem, overItem: FSItem?, replyHandler: (FSFileName?, (any Error)?) -> Void)

Renames an item from one path in the file system to another.

**Required**

func reclaimItem(FSItem, replyHandler: ((any Error)?) -> Void)

Reclaims an item, releasing any resources allocated for the item.

**Required**


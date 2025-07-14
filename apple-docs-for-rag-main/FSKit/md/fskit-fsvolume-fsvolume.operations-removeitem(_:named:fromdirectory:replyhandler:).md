

- FSKit
- FSVolume
- FSVolume.Operations
-  removeItem(\_:named:fromDirectory:replyHandler:) 

Instance Method

# removeItem(\_:named:fromDirectory:replyHandler:)

Removes an existing item from a given directory.

macOS 15.4+

``` source
func removeItem(
    _ item: FSItem,
    named name: FSFileName,
    fromDirectory directory: FSItem,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func removeItem(
    _ item: FSItem,
    named name: FSFileName,
    fromDirectory directory: FSItem
) async throws
```

**Required**

## Parameters 

`item`  

The item to remove.

`name`  

The name of the item to remove.

`directory`  

The directory from which to remove the item.

`reply`  

A block or closure to indicate success or failure. If removal fails, pass an error as the one parameter to the reply handler. If removal succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply throw an error or return normally.

## Discussion

Don’t actually remove the item object itself in your implementation; instead, only remove the given item name from the given directory. Remove and deallocate the item in reclaimItem(_:replyHandler:).

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

func lookupItem(named: FSFileName, inDirectory: FSItem, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Looks up an item within a directory.

**Required**

func renameItem(FSItem, inDirectory: FSItem, named: FSFileName, to: FSFileName, inDirectory: FSItem, overItem: FSItem?, replyHandler: (FSFileName?, (any Error)?) -> Void)

Renames an item from one path in the file system to another.

**Required**

func reclaimItem(FSItem, replyHandler: ((any Error)?) -> Void)

Reclaims an item, releasing any resources allocated for the item.

**Required**


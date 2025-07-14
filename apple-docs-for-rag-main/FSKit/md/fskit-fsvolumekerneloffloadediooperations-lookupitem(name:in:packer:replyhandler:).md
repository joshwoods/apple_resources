

- FSKit
- FSVolumeKernelOffloadedIOOperations
-  lookupItem(name:in:packer:replyHandler:) 

Instance Method

# lookupItem(name:in:packer:replyHandler:)

Looks up an item within a directory and maps its disk space.

macOS 15.4+

``` source
func lookupItem(
    name: FSFileName,
    in directory: FSItem,
    packer: FSExtentPacker,
    replyHandler reply: @escaping (FSItem?, FSFileName?, (any Error)?) -> Void
)
```

``` source
func lookupItem(
    name: FSFileName,
    in directory: FSItem,
    packer: FSExtentPacker
) async throws -> (FSItem, FSFileName)
```

**Required**

## Parameters 

`name`  

The name of the file to look up.

`directory`  

The directory in which to look up the file.

`packer`  

An extent packer you use to pack the file’s allocated disk space.

`reply`  

A block or closure to indicate success or failure. If lookup succeeds, pass the found FSItem and its FSFileName, along with a `nil` error. If lookup fails, pass the relevant error as the third parameter; FSKit ignores any FSItem or FSFileName in this case. For an `async` Swift implementation, there’s no reply handler; instead, return a tuple of the FSItem and its FSFileName or throw an error.

## Discussion

This method allows the module to opportunistically supply extents, avoiding future calls to blockmapFile(_:offset:length:flags:operationID:packer:replyHandler:). Only perform this technique opportunistically. In particular, don’t perform additional I/O to fetch extent data.

## See Also

### Working with items

func createFile(name: FSFileName, in: FSItem, attributes: FSItem.SetAttributesRequest, packer: FSExtentPacker, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Creates a new file item and map its disk space.

**Required**

class SetAttributesRequest

A request to set attributes on an item.

func preallocateSpace(for: FSItem, at: off_t, length: Int, flags: FSVolume.PreallocateFlags, packer: FSExtentPacker, replyHandler: (Int, (any Error)?) -> Void)

Preallocates and maps disk space for the given file.

struct PreallocateFlags

Behavior flags for preallocation operations.




- FSKit
- FSVolumeKernelOffloadedIOOperations
-  createFile(name:in:attributes:packer:replyHandler:) 

Instance Method

# createFile(name:in:attributes:packer:replyHandler:)

Creates a new file item and map its disk space.

macOS 15.4+

``` source
func createFile(
    name: FSFileName,
    in directory: FSItem,
    attributes: FSItem.SetAttributesRequest,
    packer: FSExtentPacker,
    replyHandler reply: @escaping (FSItem?, FSFileName?, (any Error)?) -> Void
)
```

``` source
func createFile(
    name: FSFileName,
    in directory: FSItem,
    attributes: FSItem.SetAttributesRequest,
    packer: FSExtentPacker
) async throws -> (FSItem, FSFileName)
```

**Required**

## Parameters 

`name`  

The new file’s name.

`directory`  

The directory in which to create the file.

`attributes`  

Attributes to apply to the new file.

`packer`  

An extent packer you use to pack the file’s allocated disk space.

`reply`  

A block or closure to indicate success or failure. If creation succeeds, pass the newly created FSItem and its FSFileName, along with a `nil` error. If creation fails, pass the relevant error as the third parameter; FSKit ignores any FSItem or FSFileName in this case. For an `async` Swift implementation, there’s no reply handler; instead, return a tuple of the FSItem and its FSFileName or throw an error.

## Discussion

This method allows the module to opportunistically supply extents, avoiding future calls to blockmapFile(_:offset:length:flags:operationID:packer:replyHandler:). Only perform this technique opportunistically. In particular, don’t perform additional I/O to fetch extent data.

Packing extents in this method requires that `attributes` defines a size greater than 0.

An implementation that doesn’t supply the extents can ignore the packer and call the corresponding method in the FSVolume.Operations protocol, createItem(named:type:inDirectory:attributes:replyHandler:).

## See Also

### Working with items

class SetAttributesRequest

A request to set attributes on an item.

func lookupItem(name: FSFileName, in: FSItem, packer: FSExtentPacker, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Looks up an item within a directory and maps its disk space.

**Required**

func preallocateSpace(for: FSItem, at: off_t, length: Int, flags: FSVolume.PreallocateFlags, packer: FSExtentPacker, replyHandler: (Int, (any Error)?) -> Void)

Preallocates and maps disk space for the given file.

struct PreallocateFlags

Behavior flags for preallocation operations.


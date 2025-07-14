

- FSKit
- FSVolumeKernelOffloadedIOOperations
-  preallocateSpace(for:at:length:flags:packer:replyHandler:) 

Instance Method

# preallocateSpace(for:at:length:flags:packer:replyHandler:)

Preallocates and maps disk space for the given file.

macOS 15.4+

``` source
optional func preallocateSpace(
    for file: FSItem,
    at offset: off_t,
    length: Int,
    flags: FSVolume.PreallocateFlags,
    packer: FSExtentPacker,
    replyHandler reply: @escaping (Int, (any Error)?) -> Void
)
```

``` source
optional func preallocateSpace(
    for file: FSItem,
    at offset: off_t,
    length: Int,
    flags: FSVolume.PreallocateFlags,
    packer: FSExtentPacker
) async throws -> Int
```

## Parameters 

`file`  

The item for which to preallocate space.

`offset`  

The offset from which to allocate.

`length`  

The length of the space in bytes.

`flags`  

Flags that affect the preallocation behavior.

`packer`  

An extent packer you use to pack the file’s preallocated disk space.

`reply`  

A block or closure to indicate success or failure. If preallocation succeeds, pass the amount of bytes allocated and a nil error. If preallocation fails, pass the relevant error as the second parameter; FSKit ignores any byte count in this case. For an `async` Swift implementation, there’s no reply handler; simply return the allocated byte count or throw an error.

## Discussion

This method allows the module to opportunistically supply extents, avoiding future calls to blockmapFile(_:offset:length:flags:operationID:packer:replyHandler:).

Important

Only implement this method if your file system conforms to FSVolume.PreallocateOperations.

## See Also

### Working with items

func createFile(name: FSFileName, in: FSItem, attributes: FSItem.SetAttributesRequest, packer: FSExtentPacker, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Creates a new file item and map its disk space.

**Required**

class SetAttributesRequest

A request to set attributes on an item.

func lookupItem(name: FSFileName, in: FSItem, packer: FSExtentPacker, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Looks up an item within a directory and maps its disk space.

**Required**

struct PreallocateFlags

Behavior flags for preallocation operations.


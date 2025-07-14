

- FSKit
- FSVolumeKernelOffloadedIOOperations
-  completeIO(for:offset:length:status:flags:operationID:replyHandler:) 

Instance Method

# completeIO(for:offset:length:status:flags:operationID:replyHandler:)

Completes an I/O operation for a given file.

macOS 15.4+

``` source
func completeIO(
    for file: FSItem,
    offset: off_t,
    length: Int,
    status: any Error,
    flags: FSCompleteIOFlags,
    operationID: FSOperationID,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func completeIO(
    for file: FSItem,
    offset: off_t,
    length: Int,
    status: any Error,
    flags: FSCompleteIOFlags,
    operationID: FSOperationID
) async throws
```

**Required**

## Parameters 

`file`  

The file for which the I/O operation completed.

`offset`  

The starting logical offset at which I/O started.

`length`  

The length of the I/O range (in bytes).

`status`  

Any error that occurred during the operation. If no error occurred, this parameter is `nil`.

`flags`  

Flags that affect the behavior of the complete I/O operation.

`operationID`  

A unique identifier of the blockmap call. Any value other than `0` (Objective-C) or unspecified (Swift) corresponds to a previous call to blockmapFile(_:offset:length:flags:operationID:packer:replyHandler:) with the same `operationID`.

`reply`  

A block or closure to indicate success or failure. If completing I/O fails, pass an error as the one parameter to the reply handler. If completing I/O succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply throw an error or return normally.

## Discussion

Implement this method by updating a file’s metadata, such as its size and modification time.

FSKit may call this method without an earlier call to blockmapFile(_:offset:length:flags:operationID:packer:replyHandler:). In this case, the `operationID` is `0` (Objective-C) or unspecified (Swift).

## See Also

### Performing mapped I/O

func blockmapFile(FSItem, offset: off_t, length: Int, flags: FSBlockmapFlags, operationID: FSOperationID, packer: FSExtentPacker, replyHandler: ((any Error)?) -> Void)

Maps a file’s disk space into extents, allowing the kernel to perform I/O with that space.

**Required**

struct FSBlockmapFlags

Flags that describe the behavior of a blockmap operation.

struct FSCompleteIOFlags

Flags that describe the behavior of an I/O completion operation.


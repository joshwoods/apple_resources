

- FSKit
- FSVolume
- FSVolume.ReadWriteOperations
-  read(from:at:length:into:replyHandler:) 

Instance Method

# read(from:at:length:into:replyHandler:)

Reads the contents of the given file item.

macOS 15.4+

``` source
func read(
    from item: FSItem,
    at offset: off_t,
    length: Int,
    into buffer: FSMutableFileDataBuffer,
    replyHandler reply: @escaping (Int, (any Error)?) -> Void
)
```

``` source
func read(
    from item: FSItem,
    at offset: off_t,
    length: Int,
    into buffer: FSMutableFileDataBuffer
) async throws -> Int
```

**Required**

## Parameters 

`item`  

The item from which to read. FSKit guarantees this item will be of type FSItem.ItemType.file.

`offset`  

The offset in the file from which to start reading.

`length`  

The number of bytes to read.

`buffer`  

A buffer to receive the bytes read from the file.

`reply`  

A block or closure to indicate success or failure. If reading succeeds, pass the number of bytes read and a `nil` error. If reading fails, pass the number of bytes read prior to the error along with the relevant error. For an `async` Swift implementation, there’s no reply handler; simply return the byte count or throw an error.

## Discussion

If the number of bytes requested exceeds the number of bytes available before the end of the file, then the call copies only those bytes to `buffer`. If `offset` points past the last valid byte of the file, don’t reply with an error but set `actuallyRead` to `0`.

## See Also

### Reading and writing

class FSMutableFileDataBuffer

A wrapper object for a data buffer.

func write(contents: Data, to: FSItem, at: off_t, replyHandler: (Int, (any Error)?) -> Void)

Writes contents to the given file item.

**Required**


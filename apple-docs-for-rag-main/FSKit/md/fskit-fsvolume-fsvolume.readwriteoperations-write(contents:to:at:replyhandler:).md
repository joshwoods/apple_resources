

- FSKit
- FSVolume
- FSVolume.ReadWriteOperations
-  write(contents:to:at:replyHandler:) 

Instance Method

# write(contents:to:at:replyHandler:)

Writes contents to the given file item.

macOS 15.4+

``` source
func write(
    contents: Data,
    to item: FSItem,
    at offset: off_t,
    replyHandler reply: @escaping (Int, (any Error)?) -> Void
)
```

``` source
func write(
    contents: Data,
    to item: FSItem,
    at offset: off_t
) async throws -> Int
```

**Required**

## Parameters 

`contents`  

A buffer containing the data to write to the file.

`item`  

The item to which to write. FSKit guarantees this item will be of type FSItem.ItemType.file.

`offset`  

The offset in the file from which to start writing.

`reply`  

A block or closure to indicate success or failure. If writing succeeds, pass the number of bytes written and a `nil` error. If writing fails, pass the number of bytes written prior to the error along with the relevant error. For an `async` Swift implementation, there’s no reply handler; simply return the byte count or throw an error.

## Discussion

FSKit expects this routine to allocate space in the file system to extend the file as necessary.

If the volume experiences an out-of-space condition, reply with an error of domain NSPOSIXErrorDomain and code `ENOSPC`.

## See Also

### Reading and writing

func read(from: FSItem, at: off_t, length: Int, into: FSMutableFileDataBuffer, replyHandler: (Int, (any Error)?) -> Void)

Reads the contents of the given file item.

**Required**

class FSMutableFileDataBuffer

A wrapper object for a data buffer.


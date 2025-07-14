

- FSKit
- FSBlockDeviceResource
-  write(from:startingAt:length:) 

Instance Method

# write(from:startingAt:length:)

Asynchronously writes data from from a buffer to the resource.

macOS 15.4+

``` source
func write(
    from buffer: UnsafeRawBufferPointer,
    startingAt offset: off_t,
    length: Int
) async throws -> Int
```

## Parameters 

`buffer`  

A buffer to provide the data.

`offset`  

The offset into the resource from which to start writing.

`length`  

A maximum number of bytes to write. The completion handler receives a parameter with the actual number of bytes write.

## Return Value

The number of bytes written.

## Discussion

For the write to succeed, requests must conform to any transfer requirements of the underlying resource. Disk drives typically require sector (`physicalBlockSize`) addressed operations of one or more sector-aligned offsets.

Throws

An error describing any write error. This value is `EFAULT` if `buffer` is `NULL`, or `errno` if writing to the resource failed.

## See Also

### Reading and writing data

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) throws -> Int

Synchronously reads data from the resource into a buffer.

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asychronously reads data from the resource into a buffer.

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Reads data from the resource into a buffer and executes a closure afterwards.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws -> Int

Synchronously writes data from from a buffer to the resource and executes a block afterwards.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Writes data from from a buffer to the resource and executes a closure afterwards.




- FSKit
- FSBlockDeviceResource
-  read(into:startingAt:length:completionHandler:) 

Instance Method

# read(into:startingAt:length:completionHandler:)

Reads data from the resource into a buffer and executes a closure afterwards.

macOS 15.4+

``` source
func read(
    into buffer: UnsafeMutableRawBufferPointer,
    startingAt offset: off_t,
    length: Int,
    completionHandler: @escaping (Int, (any Error)?) -> Void
)
```

## Parameters 

`buffer`  

A buffer to receive the data.

`offset`  

The offset into the resource from which to start reading.

`length`  

A maximum number of bytes to read. The completion handler receives a parameter with the actual number of bytes read.

`completionHandler`  

A closure that executes after the read operation completes. If successful, the first parameter contains the number of bytes actually read. In the case of an error, the second parameter contains a non-`nil` error. This value is `EFAULT` if `buffer` is `nil`, or `errno` if reading from the resource failed.

## Discussion

For the read to succeed, requests must conform to any transfer requirements of the underlying resource. Disk drives typically require sector (`physicalBlockSize`) addressed operations of one or more sector-aligned offsets.

## See Also

### Reading and writing data

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) throws -> Int

Synchronously reads data from the resource into a buffer.

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asychronously reads data from the resource into a buffer.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws -> Int

Synchronously writes data from from a buffer to the resource and executes a block afterwards.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asynchronously writes data from from a buffer to the resource.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Writes data from from a buffer to the resource and executes a closure afterwards.


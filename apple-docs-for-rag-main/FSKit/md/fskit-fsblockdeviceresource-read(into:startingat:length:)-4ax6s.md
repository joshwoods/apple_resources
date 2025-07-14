

- FSKit
- FSBlockDeviceResource
-  read(into:startingAt:length:) 

Instance Method

# read(into:startingAt:length:)

Synchronously reads data from the resource into a buffer.

macOS 15.4+

``` source
func read(
    into buffer: UnsafeMutableRawBufferPointer,
    startingAt offset: off_t,
    length: Int
) throws -> Int
```

## Parameters 

`buffer`  

A buffer to receive the data.

`offset`  

The offset into the resource from which to start reading.

`length`  

A maximum number of bytes to read. The method’s return value contains the actual number of bytes read.

## Return Value

The actual number of bytes read.

## Discussion

This is a synchronous version of read(into:startingAt:length:).

In some cases, this method performs a partial read. In this case, the return value is shorter than the requested length.

Throws

An error describing any read error. This value is `EFAULT` if `buffer` is `NULL`, or `errno` if reading from the resource failed.

## See Also

### Reading and writing data

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asychronously reads data from the resource into a buffer.

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Reads data from the resource into a buffer and executes a closure afterwards.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws -> Int

Synchronously writes data from from a buffer to the resource and executes a block afterwards.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asynchronously writes data from from a buffer to the resource.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Writes data from from a buffer to the resource and executes a closure afterwards.


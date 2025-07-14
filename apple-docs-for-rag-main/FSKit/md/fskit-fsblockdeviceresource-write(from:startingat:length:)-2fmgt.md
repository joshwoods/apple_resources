

- FSKit
- FSBlockDeviceResource
-  write(from:startingAt:length:) 

Instance Method

# write(from:startingAt:length:)

Synchronously writes data from from a buffer to the resource and executes a block afterwards.

macOS 15.4+

``` source
func write(
    from buffer: UnsafeRawBufferPointer,
    startingAt offset: off_t,
    length: Int
) throws -> Int
```

## Parameters 

`buffer`  

A buffer to provide the data.

`offset`  

The offset into the resource from which to start writing.

`length`  

A maximum number of bytes to write. The completion handler receives a parameter with the actual number of bytes write.

## Return Value

The actual number of bytes written.

## Discussion

This method is a synchronous version of writeFrom:startingAt:length:completionHandler:.

In some cases, this method performs a partial write. In this case, the return value is shorter than the requested length, and the `error` is set to `nil`.

Throws

Any error encountered while writing data.

## See Also

### Reading and writing data

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) throws -> Int

Synchronously reads data from the resource into a buffer.

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asychronously reads data from the resource into a buffer.

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Reads data from the resource into a buffer and executes a closure afterwards.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asynchronously writes data from from a buffer to the resource.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Writes data from from a buffer to the resource and executes a closure afterwards.


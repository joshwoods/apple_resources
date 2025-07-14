

- System
- FileDescriptor
-  write(\_:retryOnInterrupt:) 

Instance Method

# write(\_:retryOnInterrupt:)

Writes the contents of a buffer at the current file offset.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func write(
    _ buffer: UnsafeRawBufferPointer,
    retryOnInterrupt: Bool = true
) throws -> Int
```

## Parameters 

`buffer`  

The region of memory that contains the data being written.

`retryOnInterrupt`  

Whether to retry the write operation if it throws interrupted. The default is `true`. Pass `false` to try only once and throw an error upon interruption.

## Return Value

The number of bytes that were written.

## Mentioned in 

Adopting Swift File Operations

## Discussion

After writing, this method increments the file’s offset by the number of bytes written. To change the file’s offset, call the seek(offset:from:) method.

The corresponding C function is `write`.

## See Also

### Writing To A File

func write(toAbsoluteOffset: Int64, UnsafeRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Writes the contents of a buffer at the specified offset.

func writeAll&lt;S>(S) throws -> Int

Writes a sequence of bytes to the current offset and then updates the offset.

func writeAll&lt;S>(toAbsoluteOffset: Int64, S) throws -> Int

Writes a sequence of bytes to the given offset.




- System
- FileDescriptor
-  write(toAbsoluteOffset:\_:retryOnInterrupt:) 

Instance Method

# write(toAbsoluteOffset:\_:retryOnInterrupt:)

Writes the contents of a buffer at the specified offset.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func write(
    toAbsoluteOffset offset: Int64,
    _ buffer: UnsafeRawBufferPointer,
    retryOnInterrupt: Bool = true
) throws -> Int
```

## Parameters 

`offset`  

The file offset where writing begins.

`buffer`  

The region of memory that contains the data being written.

`retryOnInterrupt`  

Whether to retry the write operation if it throws interrupted. The default is `true`. Pass `false` to try only once and throw an error upon interruption.

## Return Value

The number of bytes that were written.

## Mentioned in 

Adopting Swift File Operations

## Discussion

Unlike write(_:retryOnInterrupt:), this method leaves the file’s existing offset unchanged.

The corresponding C function is `pwrite`.

## See Also

### Writing To A File

func write(UnsafeRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Writes the contents of a buffer at the current file offset.

func writeAll&lt;S>(S) throws -> Int

Writes a sequence of bytes to the current offset and then updates the offset.

func writeAll&lt;S>(toAbsoluteOffset: Int64, S) throws -> Int

Writes a sequence of bytes to the given offset.


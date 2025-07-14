

- System
- FileDescriptor
-  writeAll(\_:) 

Instance Method

# writeAll(\_:)

Writes a sequence of bytes to the current offset and then updates the offset.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@discardableResult
func writeAll(_ sequence: S) throws -> Int where S : Sequence, S.Element == UInt8
```

## Parameters 

`sequence`  

The bytes to write.

## Return Value

The number of bytes written, equal to the number of elements in `sequence`.

## Discussion

This method either writes the entire contents of `sequence`, or throws an error if only part of the content was written.

Writes to the position associated with this file descriptor, and increments that position by the number of bytes written. See also seek(offset:from:).

If `sequence` doesn’t implement the withContiguousStorageIfAvailable(_:) method, temporary space will be allocated as needed.

## See Also

### Writing To A File

func write(UnsafeRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Writes the contents of a buffer at the current file offset.

func write(toAbsoluteOffset: Int64, UnsafeRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Writes the contents of a buffer at the specified offset.

func writeAll&lt;S>(toAbsoluteOffset: Int64, S) throws -> Int

Writes a sequence of bytes to the given offset.


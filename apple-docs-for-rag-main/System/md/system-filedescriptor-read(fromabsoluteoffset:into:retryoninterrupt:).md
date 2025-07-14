

- System
- FileDescriptor
-  read(fromAbsoluteOffset:into:retryOnInterrupt:) 

Instance Method

# read(fromAbsoluteOffset:into:retryOnInterrupt:)

Reads bytes at the specified offset into a buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func read(
    fromAbsoluteOffset offset: Int64,
    into buffer: UnsafeMutableRawBufferPointer,
    retryOnInterrupt: Bool = true
) throws -> Int
```

## Parameters 

`offset`  

The file offset where reading begins.

`buffer`  

The region of memory to read into.

`retryOnInterrupt`  

Whether to retry the read operation if it throws interrupted. The default is `true`. Pass `false` to try only once and throw an error upon interruption.

## Return Value

The number of bytes that were read.

## Mentioned in 

Adopting Swift File Operations

## Discussion

The doc://com.apple.documentation/documentation/swift/unsafemutablerawbufferpointer/count-95usp property of `buffer` determines the maximum number of bytes that are read into that buffer.

Unlike read(into:retryOnInterrupt:), this method leaves the file’s existing offset unchanged.

The corresponding C function is `pread`.

## See Also

### Reading From a File

func read(into: UnsafeMutableRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Reads bytes at the current file offset into a buffer.


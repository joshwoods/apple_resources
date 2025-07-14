

- Core Media
-  CMBlockBufferFlags 

Type Alias

# CMBlockBufferFlags

A type for flags that control behaviors and features of block buffer APIs.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMBlockBufferFlags = UInt32
```

## Topics

### Constants

var kCMBlockBufferAssureMemoryNowFlag: CMBlockBufferFlags

When passed to routines that accept block allocators, causes the memory block to be allocated immediately.

var kCMBlockBufferAlwaysCopyDataFlag: CMBlockBufferFlags

Used with CMBlockBuffer to cause it to always produce an allocated copy of the desired data.

var kCMBlockBufferDontOptimizeDepthFlag: CMBlockBufferFlags

Passed to block buffers to suppress reference depth optimization.

var kCMBlockBufferPermitEmptyReferenceFlag: CMBlockBufferFlags

Passed to CMBlockBuffer and CMBlockBuffer to allow references into a `CMBlockBuffer` that may not yet be populated.

## See Also

### Creating a Block Buffer

func CMBlockBufferCreateEmpty(allocator: CFAllocator?, capacity: UInt32, flags: CMBlockBufferFlags, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Creates an empty block buffer.

func CMBlockBufferCreateWithMemoryBlock(allocator: CFAllocator?, memoryBlock: UnsafeMutableRawPointer?, blockLength: Int, blockAllocator: CFAllocator?, customBlockSource: UnsafePointer&lt;CMBlockBufferCustomBlockSource>?, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Creates a block buffer that’s backed by a memory block.

func CMBlockBufferCreateWithBufferReference(allocator: CFAllocator?, referenceBuffer: CMBlockBuffer, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Creates a block buffer that refers to another block buffer object.

func CMBlockBufferCreateContiguous(allocator: CFAllocator?, sourceBuffer: CMBlockBuffer, blockAllocator: CFAllocator?, customBlockSource: UnsafePointer&lt;CMBlockBufferCustomBlockSource>?, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Creates a block buffer that contains a contiguous copy of, or reference to, the data specified by the parameters.

Block Buffer Flags

An enumeration of flags that control behaviors and features of block buffer APIs.

struct CMBlockBufferCustomBlockSource

A structure to support custom memory allocation and deallocation for a block used in a block buffer.

Custom Block Source Version

A custom block source version identifier.


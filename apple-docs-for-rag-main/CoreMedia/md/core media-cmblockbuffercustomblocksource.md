

- Core Media
-  CMBlockBufferCustomBlockSource 

Structure

# CMBlockBufferCustomBlockSource

A structure to support custom memory allocation and deallocation for a block used in a block buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMBlockBufferCustomBlockSource
```

## Overview

This structure allows a client to provide a custom facility for obtaining the memory block to be used in a `CMBlockBuffer`. You use this structure with functions that accept a memory block allocator.

## Topics

### Initializers

init()

init(version: UInt32, AllocateBlock: ((UnsafeMutableRawPointer?, Int) -> UnsafeMutableRawPointer?)?, FreeBlock: ((UnsafeMutableRawPointer?, UnsafeMutableRawPointer, Int) -> Void)?, refCon: UnsafeMutableRawPointer?)

### Properties

var AllocateBlock: ((UnsafeMutableRawPointer?, Int) -> UnsafeMutableRawPointer?)?

The function to allocate memory.

var FreeBlock: ((UnsafeMutableRawPointer?, UnsafeMutableRawPointer, Int) -> Void)?

A function to call once when the `CMBlockBuffer` is disposed.

var refCon: UnsafeMutableRawPointer?

Contextual information passed to both the allocate and free function calls.

var version: UInt32

## Relationships

### Conforms To

- BitwiseCopyable

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

typealias CMBlockBufferFlags

A type for flags that control behaviors and features of block buffer APIs.

Block Buffer Flags

An enumeration of flags that control behaviors and features of block buffer APIs.

Custom Block Source Version

A custom block source version identifier.


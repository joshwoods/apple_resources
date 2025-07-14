

- Foundation
- Object Runtime
-  Memory Management Functions 

API Collection

# Memory Management Functions

Perform low-level memory management tasks.

## Topics

### Core Foundation ARC Integration

func CFBridgingRetain(Any?) -> CFTypeRef?

Casts an Objective-C pointer to a Core Foundation pointer and also transfers ownership to the caller.

### Memory Management

func NSAllocateMemoryPages(Int) -> UnsafeMutableRawPointer

Allocates a new block of memory.

func NSCopyMemoryPages(UnsafeRawPointer, UnsafeMutableRawPointer, Int)

Copies a block of memory.

func NSDeallocateMemoryPages(UnsafeMutableRawPointer, Int)

Deallocates the specified block of memory.

func NSLogPageSize() -> Int

Returns the binary log of the page size.

func NSPageSize() -> Int

Returns the number of bytes in a page.

func NSRealMemoryAvailable() -> Int

Returns information about the user’s system.

Deprecated

func NSRoundDownToMultipleOfPageSize(Int) -> Int

Returns the specified number of bytes rounded down to a multiple of the page size.

func NSRoundUpToMultipleOfPageSize(Int) -> Int

Returns the specified number of bytes rounded up to a multiple of the page size.

## See Also

### Memory Management


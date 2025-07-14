

- Foundation
-  NSRoundDownToMultipleOfPageSize(\_:) 

Function

# NSRoundDownToMultipleOfPageSize(\_:)

Returns the specified number of bytes rounded down to a multiple of the page size.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSRoundDownToMultipleOfPageSize(_ bytes: Int) -> Int
```

## Return Value

In bytes, the multiple of the page size that is closest to, but not greater than, `byteCount` (that is, the number of bytes rounded down to a multiple of the page size).

## See Also

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

func NSRoundUpToMultipleOfPageSize(Int) -> Int

Returns the specified number of bytes rounded up to a multiple of the page size.


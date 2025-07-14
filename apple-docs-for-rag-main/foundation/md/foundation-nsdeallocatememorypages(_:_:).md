

- Foundation
-  NSDeallocateMemoryPages(\_:\_:) 

Function

# NSDeallocateMemoryPages(\_:\_:)

Deallocates the specified block of memory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSDeallocateMemoryPages(
    _ ptr: UnsafeMutableRawPointer,
    _ bytes: Int
)
```

## Discussion

This function deallocates memory that was allocated with `NSAllocateMemoryPages`.

## See Also

### Memory Management

func NSAllocateMemoryPages(Int) -> UnsafeMutableRawPointer

Allocates a new block of memory.

func NSCopyMemoryPages(UnsafeRawPointer, UnsafeMutableRawPointer, Int)

Copies a block of memory.

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


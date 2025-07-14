

- Foundation
-  NSAllocateMemoryPages(\_:) 

Function

# NSAllocateMemoryPages(\_:)

Allocates a new block of memory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSAllocateMemoryPages(_ bytes: Int) -> UnsafeMutableRawPointer
```

## Discussion

Allocates the integral number of pages whose total size is closest to, but not less than, `byteCount`. The allocated pages are guaranteed to be filled with zeros. If the allocation fails, raises `NSInvalidArgumentException`.

## See Also

### Memory Management

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


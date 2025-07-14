

- Foundation
-  NSRealMemoryAvailable() Deprecated

Function

# NSRealMemoryAvailable()

Returns information about the user’s system.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func NSRealMemoryAvailable() -> Int
```

Deprecated

Use NSProcessInfo instead

## Return Value

The number of bytes available in RAM.

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

func NSRoundDownToMultipleOfPageSize(Int) -> Int

Returns the specified number of bytes rounded down to a multiple of the page size.

func NSRoundUpToMultipleOfPageSize(Int) -> Int

Returns the specified number of bytes rounded up to a multiple of the page size.


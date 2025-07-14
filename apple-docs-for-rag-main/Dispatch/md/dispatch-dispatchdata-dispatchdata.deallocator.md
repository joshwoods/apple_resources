

- Dispatch
- DispatchData
-  DispatchData.Deallocator 

Enumeration

# DispatchData.Deallocator

Memory deallocators for dispatch data objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum Deallocator
```

## Topics

### Deallocators

case free

Use `free` to deallocate memory.

case unmap

Use `munmap` to deallocate memory.

case custom(DispatchQueue?, () -> Void)

Use a custom deallocator.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a Dispatch Data Structure

init(bytes: UnsafeRawBufferPointer)

Creates a new dispatch data object from the specified memory buffer.

init(bytesNoCopy: UnsafeRawBufferPointer, deallocator: DispatchData.Deallocator)

Creates a new dispatch data object using the specified memory buffer and deallocator.

func withUnsafeBytes&lt;Result, ContentType>(body: (UnsafePointer&lt;ContentType>) throws -> Result) rethrows -> Result

static let empty: DispatchData

A dispatch data object representing a zero-length memory region.


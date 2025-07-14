

- Dispatch
- DispatchData
-  init(bytes:) 

Initializer

# init(bytes:)

Creates a new dispatch data object from the specified memory buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(bytes buffer: UnsafeRawBufferPointer)
```

## Parameters 

`buffer`  

A contiguous buffer of memory containing the initial data.

## See Also

### Creating a Dispatch Data Structure

init(bytesNoCopy: UnsafeRawBufferPointer, deallocator: DispatchData.Deallocator)

Creates a new dispatch data object using the specified memory buffer and deallocator.

func withUnsafeBytes&lt;Result, ContentType>(body: (UnsafePointer&lt;ContentType>) throws -> Result) rethrows -> Result

enum Deallocator

Memory deallocators for dispatch data objects.

static let empty: DispatchData

A dispatch data object representing a zero-length memory region.




- Dispatch
- DispatchData
-  empty 

Type Property

# empty

A dispatch data object representing a zero-length memory region.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let empty: DispatchData
```

## See Also

### Creating a Dispatch Data Structure

init(bytes: UnsafeRawBufferPointer)

Creates a new dispatch data object from the specified memory buffer.

init(bytesNoCopy: UnsafeRawBufferPointer, deallocator: DispatchData.Deallocator)

Creates a new dispatch data object using the specified memory buffer and deallocator.

func withUnsafeBytes&lt;Result, ContentType>(body: (UnsafePointer&lt;ContentType>) throws -> Result) rethrows -> Result

enum Deallocator

Memory deallocators for dispatch data objects.


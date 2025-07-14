

- Dispatch
- DispatchData
-  withUnsafeBytes(body:) 

Instance Method

# withUnsafeBytes(body:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func withUnsafeBytes(body: (UnsafePointer) throws -> Result) rethrows -> Result
```

## See Also

### Creating a Dispatch Data Structure

init(bytes: UnsafeRawBufferPointer)

Creates a new dispatch data object from the specified memory buffer.

init(bytesNoCopy: UnsafeRawBufferPointer, deallocator: DispatchData.Deallocator)

Creates a new dispatch data object using the specified memory buffer and deallocator.

enum Deallocator

Memory deallocators for dispatch data objects.

static let empty: DispatchData

A dispatch data object representing a zero-length memory region.


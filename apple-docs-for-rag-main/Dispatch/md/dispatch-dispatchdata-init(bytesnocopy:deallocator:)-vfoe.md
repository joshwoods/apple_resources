

- Dispatch
- DispatchData
-  init(bytesNoCopy:deallocator:) 

Initializer

# init(bytesNoCopy:deallocator:)

Creates a new dispatch data object using the specified memory buffer and deallocator.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    bytesNoCopy bytes: UnsafeRawBufferPointer,
    deallocator: DispatchData.Deallocator = .free
)
```

## Parameters 

`bytes`  

A contiguous buffer of memory containing the initial data.

`deallocator`  

The deallocator responsible for releasing the memory associated with the data object. For a list of possible options, see DispatchData.Deallocator.

## See Also

### Creating a Dispatch Data Structure

init(bytes: UnsafeRawBufferPointer)

Creates a new dispatch data object from the specified memory buffer.

func withUnsafeBytes&lt;Result, ContentType>(body: (UnsafePointer&lt;ContentType>) throws -> Result) rethrows -> Result

enum Deallocator

Memory deallocators for dispatch data objects.

static let empty: DispatchData

A dispatch data object representing a zero-length memory region.




- Dispatch
- DispatchData
-  init(bytesNoCopy:deallocator:) 

Initializer

# init(bytesNoCopy:deallocator:)

Initialize a data object without copying the bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwiftDeprecated

``` source
init(
    bytesNoCopy bytes: UnsafeBufferPointer,
    deallocator: DispatchData.Deallocator = .free
)
```

## Parameters 

`bytes`  

A pointer to the bytes.

`deallocator`  

Specifies the mechanism to free the indicated buffer.

## See Also

### Deprecated

init(bytes: UnsafeBufferPointer&lt;UInt8>)

Initialize a data object with copied memory content.

func append(UnsafePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;DispatchData.Index>)


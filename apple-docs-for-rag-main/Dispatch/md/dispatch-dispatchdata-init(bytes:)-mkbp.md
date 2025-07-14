

- Dispatch
- DispatchData
-  init(bytes:) 

Initializer

# init(bytes:)

Initialize a data object with copied memory content.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwiftDeprecated

``` source
init(bytes buffer: UnsafeBufferPointer)
```

## Parameters 

`buffer`  

A pointer to the memory. It will be copied.

## See Also

### Deprecated

init(bytesNoCopy: UnsafeBufferPointer&lt;UInt8>, deallocator: DispatchData.Deallocator)

Initialize a data object without copying the bytes.

func append(UnsafePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;DispatchData.Index>)


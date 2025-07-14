

- FSKit
- FSMutableFileDataBuffer
-  withUnsafeMutableBytes(\_:) 

Instance Method

# withUnsafeMutableBytes(\_:)

Performs the given closure with an unsafe pointer to the underlying bytes of the data buffer.

macOS 15.4+

``` source
func withUnsafeMutableBytes(_ body: (UnsafeMutableRawBufferPointer) throws(E) -> R) throws(E) -> R where E : Error
```

## Parameters 

`body`  

The closure to perform with the pointer.

## See Also

### Accessing buffer properties

var length: Int

The data length of the buffer.


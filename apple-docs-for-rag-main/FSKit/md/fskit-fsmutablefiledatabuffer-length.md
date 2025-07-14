

- FSKit
- FSMutableFileDataBuffer
-  length 

Instance Property

# length

The data length of the buffer.

macOS 15.4+

``` source
var length: Int { get }
```

## See Also

### Accessing buffer properties

func withUnsafeMutableBytes&lt;R, E>((UnsafeMutableRawBufferPointer) throws(E) -> R) throws(E) -> R

Performs the given closure with an unsafe pointer to the underlying bytes of the data buffer.


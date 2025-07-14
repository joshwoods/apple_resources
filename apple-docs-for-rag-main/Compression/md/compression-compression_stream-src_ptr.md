

- Compression
- compression_stream
-  src_ptr 

Instance Property

# src_ptr

A pointer to the first byte of the source buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var src_ptr: UnsafePointer
```

## See Also

### Compression Stream Properties

var dst_ptr: UnsafeMutablePointer&lt;UInt8>

A pointer to the first byte of the destination buffer.

var dst_size: Int

The size, in bytes, of the destination buffer.

var src_size: Int

The size, in bytes, of the source buffer.

var state: UnsafeMutableRawPointer?

The stream state object of the compression stream.


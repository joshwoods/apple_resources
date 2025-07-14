

- Compression
- compression_stream
-  init(dst_ptr:dst_size:src_ptr:src_size:state:) 

Initializer

# init(dst_ptr:dst_size:src_ptr:src_size:state:)

Returns a new compression stream structure.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    dst_ptr: UnsafeMutablePointer,
    dst_size: Int,
    src_ptr: UnsafePointer,
    src_size: Int,
    state: UnsafeMutableRawPointer?
)
```

## Parameters 

`dst_ptr`  

A pointer to the first byte of the destination buffer.

`dst_size`  

The size, in bytes, on the destination buffer.

`src_ptr`  

A pointer to the first byte of the source buffer.

`src_size`  

The size, in bytes, on the source buffer.

`state`  

The stream state object of the compression stream. You should not directly access this field.


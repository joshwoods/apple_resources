

- SceneKit
- SCNBufferStream
-  writeBytes(\_:count:) 

Instance Method

# writeBytes(\_:count:)

Copies the specified data bytes into the underlying Metal buffer for use by a shader.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func writeBytes(
    _ bytes: UnsafeRawPointer,
    count length: Int
)
```

**Required**

## Parameters 

`bytes`  

The memory address from which to copy data.

`length`  

The number of bytes to copy into the Metal buffer.


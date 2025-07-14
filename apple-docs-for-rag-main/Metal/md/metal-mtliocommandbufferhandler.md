

- Metal
-  MTLIOCommandBufferHandler 

Type Alias

# MTLIOCommandBufferHandler

A convenience type that defines the signature of an input/output command buffer’s completion handler.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLIOCommandBufferHandler = (any MTLIOCommandBuffer) -> Void
```

## Parameters 

`inputOutputCommandBuffer`  

The MTLIOCommandBuffer instance that has finished executing is calling your completion handler.

## See Also

### I/O Command Buffers

protocol MTLIOCommandBuffer

A command buffer that contains input/output commands that work with files in the file systems and Metal resources.

protocol MTLIOFileHandle

Represents a raw or compressed file, such as a resource asset file in your app’s bundle.

enum MTLIOStatus

Represents the state of an input/output command buffer.

enum Code

The error codes for creating an input/output file handle.

let MTLIOErrorDomain: String

The domain for input/output command queue errors.


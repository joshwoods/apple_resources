

- Core Foundation
-  CFStreamCreateBoundPair(\_:\_:\_:\_:) 

Function

# CFStreamCreateBoundPair(\_:\_:\_:\_:)

Creates a bound pair of read and write streams.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStreamCreateBoundPair(
    _ alloc: CFAllocator!,
    _ readStream: UnsafeMutablePointer?>!,
    _ writeStream: UnsafeMutablePointer?>!,
    _ transferBufferSize: CFIndex
)
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new objects. Pass kCFAllocatorDefault or `NULL` to use the current default allocator.

`readStream`  

On return, contains a readable stream. Ownership follows the The Create Rule.

`writeStream`  

On return, contains a writable stream. Ownership follows the The Create Rule.

`transferBufferSize`  

The size of the buffer, in bytes, used to transfer data from `readStream` to `writeStream`.

## Discussion

The created streams are bound to one another, such that any data written to `writeStream` is received by `readStream`.

## See Also

### Related Documentation

class func getBoundStreams(withBufferSize: Int, inputStream: AutoreleasingUnsafeMutablePointer&lt;InputStream?>?, outputStream: AutoreleasingUnsafeMutablePointer&lt;OutputStream?>?)

Creates and returns by reference a bound pair of input and output streams.

### Creating Streams

func CFStreamCreatePairWithPeerSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!)

Creates readable and writable streams connected to a socket.

Deprecated

func CFStreamCreatePairWithSocketToHost(CFAllocator!, CFString!, UInt32, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!)

Creates readable and writable streams connected to a TCP/IP port of a particular host.

Deprecated

func CFStreamCreatePairWithSocket(CFAllocator!, CFSocketNativeHandle, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!)

Creates readable and writable streams connected to a socket.

Deprecated

func CFStreamCreatePairWithSocketToCFHost(_ alloc: CFAllocator?, _ host: CFHost, _ port: Int32, _ readStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>?, _ writeStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>?)

Creates readable and writable streams connected to a given \`CFHost\` object.

Deprecated

func CFStreamCreatePairWithSocketToNetService(_ alloc: CFAllocator?, _ service: CFNetService, _ readStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>?, _ writeStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>?)

Creates a pair of streams for a CFNetService.

Deprecated


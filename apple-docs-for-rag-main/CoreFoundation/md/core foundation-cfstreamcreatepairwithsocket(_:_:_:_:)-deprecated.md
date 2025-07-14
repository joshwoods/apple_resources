

- Core Foundation
-  CFStreamCreatePairWithSocket(\_:\_:\_:\_:) Deprecated

Function

# CFStreamCreatePairWithSocket(\_:\_:\_:\_:)

Creates readable and writable streams connected to a socket.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.1–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
func CFStreamCreatePairWithSocket(
    _ alloc: CFAllocator!,
    _ sock: CFSocketNativeHandle,
    _ readStream: UnsafeMutablePointer?>!,
    _ writeStream: UnsafeMutablePointer?>!
)
```

Deprecated

Use nw_connection_t in Network framework instead

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new objects. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`sock`  

The pre-existing (and already connected) socket which the socket streams should use.

Important

By default, your app is responsible for closing this socket after you close both streams. If you want CFNetwork to take ownership of the socket, set the kCFStreamPropertyShouldCloseNativeSocket property of the stream to kCFBooleanTrue.

`readStream`  

Upon return, a readable stream connected to the socket address in `signature`. If you pass `NULL`, this function will not create a readable stream. Ownership follows the The Create Rule.

`writeStream`  

Upon return, a writable stream connected to the socket address in `signature`. If you pass `NULL`, this function will not create a writable stream. Ownership follows the The Create Rule.

## Discussion

Most properties are shared by both streams. Setting a shared property for one stream automatically sets the property for the other.

## See Also

### Creating Streams

func CFStreamCreatePairWithPeerSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!)

Creates readable and writable streams connected to a socket.

Deprecated

func CFStreamCreatePairWithSocketToHost(CFAllocator!, CFString!, UInt32, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!)

Creates readable and writable streams connected to a TCP/IP port of a particular host.

Deprecated

func CFStreamCreateBoundPair(CFAllocator!, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!, CFIndex)

Creates a bound pair of read and write streams.

func CFStreamCreatePairWithSocketToCFHost(_ alloc: CFAllocator?, _ host: CFHost, _ port: Int32, _ readStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>?, _ writeStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>?)

Creates readable and writable streams connected to a given \`CFHost\` object.

Deprecated

func CFStreamCreatePairWithSocketToNetService(_ alloc: CFAllocator?, _ service: CFNetService, _ readStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>?, _ writeStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>?)

Creates a pair of streams for a CFNetService.

Deprecated


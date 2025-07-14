

- Dispatch
- DispatchIO
-  init(type:io:queue:cleanupHandler:) 

Initializer

# init(type:io:queue:cleanupHandler:)

Creates a new I/O channel from an existing I/O channel.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    type: DispatchIO.StreamType,
    io: DispatchIO,
    queue: DispatchQueue,
    cleanupHandler: @escaping (Int32) -> Void
)
```

## Parameters 

`type`  

The access semantics for the channel. For a list of possible values, see DispatchIO.StreamType.

`io`  

An existing channel.

`queue`  

The dispatch queue on which to perform work.

`cleanupHandler`  

The handler to execute once the channel is closed. This block has no return value and takes the following parameter:

error  
An `errno` condition if creating or opening the channel failed; otherwise, the value is `0`.

## See Also

### Creating a Dispatch I/O Object

convenience init(type: DispatchIO.StreamType, fileDescriptor: Int32, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel that accesses the specified file descriptor.

convenience init?(type: DispatchIO.StreamType, path: UnsafePointer&lt;Int8>, oflag: Int32, mode: mode_t, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel that accesses the file at the specified path, potentially creating that file in the process.

enum StreamType

The semantics for accessing the contents of a file descriptor.


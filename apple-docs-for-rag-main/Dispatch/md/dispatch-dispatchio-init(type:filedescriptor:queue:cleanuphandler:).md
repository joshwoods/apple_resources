

- Dispatch
- DispatchIO
-  init(type:fileDescriptor:queue:cleanupHandler:) 

Initializer

# init(type:fileDescriptor:queue:cleanupHandler:)

Creates a new I/O channel that accesses the specified file descriptor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    type: DispatchIO.StreamType,
    fileDescriptor: Int32,
    queue: DispatchQueue,
    cleanupHandler: @escaping (Int32) -> Void
)
```

## Parameters 

`type`  

The access semantics for the channel. For a list of possible values, see DispatchIO.StreamType.

`fileDescriptor`  

The file descriptor from which to read or write data.

`queue`  

The dispatch queue on which to perform work.

`cleanupHandler`  

The handler to execute once the channel is closed. This block has no return value and takes the following parameter:

error  
An `errno` condition if creating or opening the channel failed; otherwise, the value is `0`.

## Discussion

The channel takes control of the specified file descriptor until the channel closes, either deliberately on your part or because an error occurred. While the channel owns the file descriptor, the system modifies flags such as `O_NONBLOCK` automatically. It is a programmer error for you to modify the file descriptor while the channel owns it. However, you may create additional channels based on the same file descriptor.

## See Also

### Creating a Dispatch I/O Object

convenience init?(type: DispatchIO.StreamType, path: UnsafePointer&lt;Int8>, oflag: Int32, mode: mode_t, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel that accesses the file at the specified path, potentially creating that file in the process.

convenience init(type: DispatchIO.StreamType, io: DispatchIO, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel from an existing I/O channel.

enum StreamType

The semantics for accessing the contents of a file descriptor.


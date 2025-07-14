

- Dispatch
- DispatchIO
-  read(fromFileDescriptor:maxLength:runningHandlerOn:handler:) 

Type Method

# read(fromFileDescriptor:maxLength:runningHandlerOn:handler:)

Schedules an asynchronous read operation using the specified file descriptor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func read(
    fromFileDescriptor: Int32,
    maxLength: Int,
    runningHandlerOn queue: DispatchQueue,
    handler: @escaping (DispatchData, Int32) -> Void
)
```

## Parameters 

`fromFileDescriptor`  

The file descriptor from which to read the data.

`maxLength`  

The maximum number of bytes to read from the channel. Specify `SIZE_MAX` to continue reading data until an EOF is reached.

`queue`  

The dispatch queue on which to submit the `handler` block.

`handler`  

The handler to execute once the channel is closed. This block has no return value and takes the following parameters:

data  
A DispatchData object containing the data read from the file descriptor.

error  
An `errno` condition if there was an error; otherwise, the value is `0`.

## Discussion

This is a convenience method for initiating a single, asynchronous read operation from the current position of the specified file descriptor. This method is intended for simple operations where you do not need the overhead of creating a channel and do not plan on issuing more than a few calls to read or write data. Once submitted, there is no way to cancel the read operation.

After calling this method, the system takes control of the specified file descriptor until the handler block is enqueued. While it controls the file descriptor, the system may modify it on behalf of the application. For example, the system typically adds the `O_NONBLOCK` flag to ensure that any operations are non-blocking. During that time, it is an error for your application to modify the file descriptor directly. However, you may pass the file descriptor to this method or the dispatch_write function to perform additional reads or writes. You may also use the file descriptor to create a new dispatch I/O channel.

The handler you provide is not queued for execution until the read operation finishes. In addition, if you issue multiple read or write calls for the same file descriptor using the convenience APIs, all of those operations must complete before any of the associated handlers are queued. If you are already using the file descriptor with another channel, use the read(offset:length:queue:ioHandler:) method to read data from the channel instead of this method.

If you attempt to read past the end of file, your handler is passed an empty data object and an error code of 0. For other types of unrecoverable errors, an appropriate error code is returned along with whatever data was read before the error occurred.

## See Also

### Reading from the File

func read(offset: off_t, length: Int, queue: DispatchQueue, ioHandler: (Bool, DispatchData?, Int32) -> Void)

Schedules an asynchronous read operation on the specified channel.


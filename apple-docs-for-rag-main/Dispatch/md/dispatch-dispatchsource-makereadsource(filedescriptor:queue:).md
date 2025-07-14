

- Dispatch
- DispatchSource
-  makeReadSource(fileDescriptor:queue:) 

Type Method

# makeReadSource(fileDescriptor:queue:)

Creates a new dispatch source object for reading bytes from the specified file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeReadSource(
    fileDescriptor: Int32,
    queue: DispatchQueue? = nil
) -> any DispatchSourceRead
```

## Parameters 

`fileDescriptor`  

A file descriptor pointing to an open file or socket. The dispatch source begins reading at the file descriptor’s current location.

`queue`  

The dispatch queue to which to execute the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceRead protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

As the system reads the contents of the file or socket, it calls your event handler to process the bytes.

## See Also

### Creating a File System Source

class func makeWriteSource(fileDescriptor: Int32, queue: DispatchQueue?) -> any DispatchSourceWrite

Creates a new dispatch source object for writing data to the specified file.

class func makeFileSystemObjectSource(fileDescriptor: Int32, eventMask: DispatchSource.FileSystemEvent, queue: DispatchQueue?) -> any DispatchSourceFileSystemObject

Creates a new dispatch source object for monitoring file-system events.

protocol DispatchSourceRead

A dispatch source object for reading data from a file descriptor.

protocol DispatchSourceWrite

A dispatch source object for writing data to a file descriptor.

protocol DispatchSourceFileSystemObject

A dispatch source that monitors events associated with a file descriptor.

struct FileSystemEvent

Events involving a change to a file system object.


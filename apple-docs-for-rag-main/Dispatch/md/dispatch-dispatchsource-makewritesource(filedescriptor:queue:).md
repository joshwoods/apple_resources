

- Dispatch
- DispatchSource
-  makeWriteSource(fileDescriptor:queue:) 

Type Method

# makeWriteSource(fileDescriptor:queue:)

Creates a new dispatch source object for writing data to the specified file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeWriteSource(
    fileDescriptor: Int32,
    queue: DispatchQueue? = nil
) -> any DispatchSourceWrite
```

## Parameters 

`fileDescriptor`  

A file descriptor pointing to an open file or socket. The dispatch source begins writing at the file descriptor’s current location.

`queue`  

The dispatch queue to use when executing the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceWrite protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

## See Also

### Creating a File System Source

class func makeReadSource(fileDescriptor: Int32, queue: DispatchQueue?) -> any DispatchSourceRead

Creates a new dispatch source object for reading bytes from the specified file.

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


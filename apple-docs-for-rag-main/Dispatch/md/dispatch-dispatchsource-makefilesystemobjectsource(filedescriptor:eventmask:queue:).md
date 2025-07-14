

- Dispatch
- DispatchSource
-  makeFileSystemObjectSource(fileDescriptor:eventMask:queue:) 

Type Method

# makeFileSystemObjectSource(fileDescriptor:eventMask:queue:)

Creates a new dispatch source object for monitoring file-system events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeFileSystemObjectSource(
    fileDescriptor: Int32,
    eventMask: DispatchSource.FileSystemEvent,
    queue: DispatchQueue? = nil
) -> any DispatchSourceFileSystemObject
```

## Parameters 

`fileDescriptor`  

A file descriptor pointing to an open file or socket.

`eventMask`  

The set of events you want to monitor. For a list of possible values, see DispatchSource.FileSystemEvent.

`queue`  

The dispatch queue to use when executing the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceFileSystemObject protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

## See Also

### Creating a File System Source

class func makeReadSource(fileDescriptor: Int32, queue: DispatchQueue?) -> any DispatchSourceRead

Creates a new dispatch source object for reading bytes from the specified file.

class func makeWriteSource(fileDescriptor: Int32, queue: DispatchQueue?) -> any DispatchSourceWrite

Creates a new dispatch source object for writing data to the specified file.

protocol DispatchSourceRead

A dispatch source object for reading data from a file descriptor.

protocol DispatchSourceWrite

A dispatch source object for writing data to a file descriptor.

protocol DispatchSourceFileSystemObject

A dispatch source that monitors events associated with a file descriptor.

struct FileSystemEvent

Events involving a change to a file system object.


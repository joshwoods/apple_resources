

- Dispatch
-  DispatchSourceFileSystemObject 

Protocol

# DispatchSourceFileSystemObject

A dispatch source that monitors events associated with a file descriptor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol DispatchSourceFileSystemObject : DispatchSourceProtocol, Sendable
```

## Overview

You do not adopt this protocol in your objects. Instead, use the makeFileSystemObjectSource(fileDescriptor:eventMask:queue:) method to create an object that adopts this protocol.

## Topics

### Getting the Data Handle

var handle: Int32

The file descriptor of the file or socket.

### Getting the Event Data

var data: DispatchSource.FileSystemEvent

The type of the last file system event.

var mask: DispatchSource.FileSystemEvent

The file descriptor attributes being monitored by the dispatch source.

## Relationships

### Inherits From

- DispatchSourceProtocol
- NSObjectProtocol
- Sendable

### Conforming Types

- DispatchSource

## See Also

### Creating a File System Source

class func makeReadSource(fileDescriptor: Int32, queue: DispatchQueue?) -> any DispatchSourceRead

Creates a new dispatch source object for reading bytes from the specified file.

class func makeWriteSource(fileDescriptor: Int32, queue: DispatchQueue?) -> any DispatchSourceWrite

Creates a new dispatch source object for writing data to the specified file.

class func makeFileSystemObjectSource(fileDescriptor: Int32, eventMask: DispatchSource.FileSystemEvent, queue: DispatchQueue?) -> any DispatchSourceFileSystemObject

Creates a new dispatch source object for monitoring file-system events.

protocol DispatchSourceRead

A dispatch source object for reading data from a file descriptor.

protocol DispatchSourceWrite

A dispatch source object for writing data to a file descriptor.

struct FileSystemEvent

Events involving a change to a file system object.


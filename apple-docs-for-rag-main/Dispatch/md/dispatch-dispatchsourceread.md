

- Dispatch
-  DispatchSourceRead 

Protocol

# DispatchSourceRead

A dispatch source object for reading data from a file descriptor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol DispatchSourceRead : DispatchSourceProtocol, Sendable
```

## Overview

You do not adopt this protocol in your objects. Instead, use the makeReadSource(fileDescriptor:queue:) method to create an object that adopts this protocol.

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

protocol DispatchSourceWrite

A dispatch source object for writing data to a file descriptor.

protocol DispatchSourceFileSystemObject

A dispatch source that monitors events associated with a file descriptor.

struct FileSystemEvent

Events involving a change to a file system object.


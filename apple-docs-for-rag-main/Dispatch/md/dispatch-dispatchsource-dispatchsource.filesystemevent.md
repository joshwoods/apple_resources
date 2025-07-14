

- Dispatch
- DispatchSource
-  DispatchSource.FileSystemEvent 

Structure

# DispatchSource.FileSystemEvent

Events involving a change to a file system object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct FileSystemEvent
```

## Topics

### File System Event Flags

static let all: DispatchSource.FileSystemEvent

All changes related to the file system object.

static let attrib: DispatchSource.FileSystemEvent

Changes to the metadata of the file system object.

static let delete: DispatchSource.FileSystemEvent

The deletion of the file system object.

static let extend: DispatchSource.FileSystemEvent

Changes to the size of the file system object.

static let funlock: DispatchSource.FileSystemEvent

The unlocking of the file system object.

static let link: DispatchSource.FileSystemEvent

Changes to the link count of the file system object.

static let rename: DispatchSource.FileSystemEvent

Changes to the name of the file system object.

static let revoke: DispatchSource.FileSystemEvent

The revocation of the file system object.

static let write: DispatchSource.FileSystemEvent

The writing of data to the file system object.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

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

protocol DispatchSourceFileSystemObject

A dispatch source that monitors events associated with a file descriptor.


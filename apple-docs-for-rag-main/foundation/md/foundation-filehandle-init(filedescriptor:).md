

- Foundation
- FileHandle
-  init(fileDescriptor:) 

Initializer

# init(fileDescriptor:)

Creates and returns a file handle object associated with the specified file descriptor.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(fileDescriptor fd: Int32)
```

## Parameters 

`fd`  

The POSIX file descriptor with which to initialize the file handle. This descriptor represents an open file or socket that you created previously. For example, when creating a file handle for a socket, you’d pass the value returned by the socket function.

## Return Value

A file handle initialized with `fileDescriptor`.

## Discussion

The file descriptor you pass in to this method isn’t owned by the file handle object. Therefore, you’re responsible for closing the file descriptor at some point after disposing of the file handle object.

You can create a file handle for a socket by using the result of a `socket` call as `fileDescriptor`.

## See Also

### Related Documentation

func closeFile()

Disallows further access to the represented file or communications channel and signals end of file on communications channels that permit writing.

Deprecated

### Creating a File Handle

init(fileDescriptor: Int32, closeOnDealloc: Bool)

Creates and returns a file handle object associated with the specified file descriptor and deallocation policy.

convenience init?(forReadingAtPath: String)

Returns a file handle initialized for reading the file, device, or named socket at the specified path.

convenience init(forReadingFromURL: URL) throws

Returns a file handle initialized for reading the file, device, or named socket at the specified URL.

convenience init?(forWritingAtPath: String)

Returns a file handle initialized for writing to the file, device, or named socket at the specified path.

convenience init(forWritingToURL: URL) throws

Returns a file handle initialized for writing to the file, device, or named socket at the specified URL.

convenience init?(forUpdatingAtPath: String)

Returns a file handle initialized for reading and writing to the file, device, or named socket at the specified path.

convenience init(forUpdatingURL: URL) throws

Returns a file handle initialized for reading and writing to the file, device, or named socket at the specified URL.

init?(coder: NSCoder)

Returns a file handle initialized from data in an unarchiver.


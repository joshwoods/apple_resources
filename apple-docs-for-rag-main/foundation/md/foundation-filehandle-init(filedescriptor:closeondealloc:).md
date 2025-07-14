

- Foundation
- FileHandle
-  init(fileDescriptor:closeOnDealloc:) 

Initializer

# init(fileDescriptor:closeOnDealloc:)

Creates and returns a file handle object associated with the specified file descriptor and deallocation policy.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    fileDescriptor fd: Int32,
    closeOnDealloc closeopt: Bool
)
```

## Parameters 

`fd`  

The POSIX file descriptor with which to initialize the file handle.

`closeopt`  

true if the returned file handle object should take ownership of the file descriptor and close it for you or false if you want to maintain ownership of the file descriptor.

## Return Value

An initialized file handle object.

## Discussion

If `flag` is false, the file descriptor you pass in to this method isn’t owned by the file handle object. In such a case, you’re responsible for closing the file descriptor at some point after disposing of the file handle object. If you want the file handle object to close the descriptor for you automatically, pass true for the `flag` parameter.

## See Also

### Related Documentation

func closeFile()

Disallows further access to the represented file or communications channel and signals end of file on communications channels that permit writing.

Deprecated

### Creating a File Handle

convenience init(fileDescriptor: Int32)

Creates and returns a file handle object associated with the specified file descriptor.

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


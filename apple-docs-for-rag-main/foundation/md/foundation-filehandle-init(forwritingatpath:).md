

- Foundation
- FileHandle
-  init(forWritingAtPath:) 

Initializer

# init(forWritingAtPath:)

Returns a file handle initialized for writing to the file, device, or named socket at the specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(forWritingAtPath path: String)
```

## Parameters 

`path`  

The path to the file, device, or named socket to access.

## Return Value

The initialized file handle object or `nil` if no file exists at `path`.

## Discussion

The file pointer is set to the beginning of the file. You cannot read data from the returned file handle object. Use the write(_:) method to write data to the file handle.

When using this method to create a file handle object, the file handle owns its associated file descriptor and is responsible for closing it.

## See Also

### Related Documentation

func write(Data)

Writes the specified data synchronously to the file handle.

Deprecated

### Creating a File Handle

convenience init(fileDescriptor: Int32)

Creates and returns a file handle object associated with the specified file descriptor.

init(fileDescriptor: Int32, closeOnDealloc: Bool)

Creates and returns a file handle object associated with the specified file descriptor and deallocation policy.

convenience init?(forReadingAtPath: String)

Returns a file handle initialized for reading the file, device, or named socket at the specified path.

convenience init(forReadingFromURL: URL) throws

Returns a file handle initialized for reading the file, device, or named socket at the specified URL.

convenience init(forWritingToURL: URL) throws

Returns a file handle initialized for writing to the file, device, or named socket at the specified URL.

convenience init?(forUpdatingAtPath: String)

Returns a file handle initialized for reading and writing to the file, device, or named socket at the specified path.

convenience init(forUpdatingURL: URL) throws

Returns a file handle initialized for reading and writing to the file, device, or named socket at the specified URL.

init?(coder: NSCoder)

Returns a file handle initialized from data in an unarchiver.


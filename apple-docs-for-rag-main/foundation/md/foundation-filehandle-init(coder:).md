

- Foundation
- FileHandle
-  init(coder:) 

Initializer

# init(coder:)

Returns a file handle initialized from data in an unarchiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(coder: NSCoder)
```

## See Also

### Creating a File Handle

convenience init(fileDescriptor: Int32)

Creates and returns a file handle object associated with the specified file descriptor.

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


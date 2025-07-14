

- Foundation
- FileHandle
-  init(forReadingFromURL:) 

Initializer

# init(forReadingFromURL:)

Returns a file handle initialized for reading the file, device, or named socket at the specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(forReadingFromURL url: URL) throws
```

``` source
convenience init(forReadingFrom url: URL) throws
```

## Parameters 

`url`  

The URL of the file, device, or named socket to access.

## Return Value

The initialized file handle object or `nil` if no file exists at `url`.

## Discussion

The file pointer is set to the beginning of the file. You cannot write data to the returned file handle object. Use the readDataToEndOfFile() or readData(ofLength:) methods to read data from it.

When using this method to create a file handle object, the file handle owns its associated file descriptor and is responsible for closing it.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

var availableData: Data

The data currently available in the receiver.

func readData(ofLength: Int) -> Data

Reads data synchronously up to the specified number of bytes.

Deprecated

func readDataToEndOfFile() -> Data

Reads the available data synchronously up to the end of file or maximum number of bytes.

Deprecated

### Creating a File Handle

convenience init(fileDescriptor: Int32)

Creates and returns a file handle object associated with the specified file descriptor.

init(fileDescriptor: Int32, closeOnDealloc: Bool)

Creates and returns a file handle object associated with the specified file descriptor and deallocation policy.

convenience init?(forReadingAtPath: String)

Returns a file handle initialized for reading the file, device, or named socket at the specified path.

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


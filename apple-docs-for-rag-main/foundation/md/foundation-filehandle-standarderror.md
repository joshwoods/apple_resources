

- Foundation
- FileHandle
-  standardError 

Type Property

# standardError

The file handle associated with the standard error file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var standardError: FileHandle { get }
```

## Return Value

The shared file handle associated with the standard error file.

## Discussion

Conventionally this is a terminal device where the system sends error messages. There’s one standard error file handle per process; it’s a shared instance.

When using this method to create a file handle object, the file handle owns its associated file descriptor and is responsible for closing it.

## See Also

### Related Documentation

convenience init(fileDescriptor: Int32)

Creates and returns a file handle object associated with the specified file descriptor.

### Getting a File Handle

class var standardInput: FileHandle

The file handle associated with the standard input file.

class var standardOutput: FileHandle

The file handle associated with the standard output file.

class var nullDevice: FileHandle

The file handle associated with a null device.


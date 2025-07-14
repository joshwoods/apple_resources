

- Foundation
- Pipe
-  fileHandleForReading 

Instance Property

# fileHandleForReading

The receiver’s read file handle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var fileHandleForReading: FileHandle { get }
```

## Discussion

The descriptor represented by this object is deleted, and the object itself is automatically deallocated when the receiver is deallocated.

You use the returned file handle to read from the pipe using `NSFileHandle`’s read methods—availableData, readDataToEndOfFile(), and readData(ofLength:).

You don’t need to send closeFile() to this object or explicitly release the object after you have finished using it.

## See Also

### Getting the File Handles for a Pipe

var fileHandleForWriting: FileHandle

The receiver’s write file handle.


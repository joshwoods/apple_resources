

- Virtualization
- VZFileHandleSerialPortAttachment
-  fileHandleForWriting 

Instance Property

# fileHandleForWriting

The file handle that the guest operating system uses to write data.

macOS 11.0+

``` source
var fileHandleForWriting: FileHandle? { get }
```

## Discussion

When you want to receive data from the guest operating system, read data from the file handle in this property.

## See Also

### Getting the file handles

var fileHandleForReading: FileHandle?

The file handle that the guest operating system uses to read data.


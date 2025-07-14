

- Virtualization
- VZFileHandleSerialPortAttachment
-  fileHandleForReading 

Instance Property

# fileHandleForReading

The file handle that the guest operating system uses to read data.

macOS 11.0+

``` source
var fileHandleForReading: FileHandle? { get }
```

## Discussion

When you want to send data to the guest operating system, write data to the file handle in this property.

## See Also

### Getting the file handles

var fileHandleForWriting: FileHandle?

The file handle that the guest operating system uses to write data.


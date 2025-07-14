

- Virtualization
- VZFileHandleSerialPortAttachment
-  init(fileHandleForReading:fileHandleForWriting:) 

Initializer

# init(fileHandleForReading:fileHandleForWriting:)

Creates a serial port attachment object from the specified file handles.

macOS 11.0+

``` source
init(
    fileHandleForReading: FileHandle?,
    fileHandleForWriting: FileHandle?
)
```

## Parameters 

`fileHandleForReading`  

The file handle that the guest operating system uses to read data. Your virtual machine writes data to this file handle. If the file descriptor for the file handle is invalid, this method raises an exception.

`fileHandleForWriting`  

The file handle to which the guest operating system writes data. Your virtual machine reads data from this file handle. If its file descriptor for the file handle is invalid, this method raises an exception.

## Return Value

A serial port attachment object.


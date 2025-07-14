

- Virtualization
- VZFileHandleNetworkDeviceAttachment
-  init(fileHandle:) 

Initializer

# init(fileHandle:)

Creates the attachment from a file handle that contains a connected datagram socket.

macOS 11.0+

``` source
init(fileHandle: FileHandle)
```

## Parameters 

`fileHandle`  

A file handle to a connected datagram socket.

## Return Value

An attachment object for the specified file handle.


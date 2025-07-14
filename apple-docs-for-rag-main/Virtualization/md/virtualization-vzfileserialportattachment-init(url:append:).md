

- Virtualization
- VZFileSerialPortAttachment
-  init(url:append:) 

Initializer

# init(url:append:)

Creates a file-based serial port attachment object.

macOS 11.0+

``` source
init(
    url: URL,
    append shouldAppend: Bool
) throws
```

## Parameters 

`url`  

The URL of a file on the local file system. The specified file must be writable by the virtual machine.

`shouldAppend`  

A Boolean that indicates whether the virtual machine opens the file in append mode. Specify true to append data to the file, and specify false to replace the contents of the file with any new data.

## Return Value

A file-based serial port attachment on success, or `nil` if initialization failed.




- Virtualization
- VZFileSerialPortAttachment
-  append 

Instance Property

# append

A Boolean that indicates whether the virtual machine appends data to the file.

macOS 11.0+

``` source
var append: Bool { get }
```

## Discussion

When the value of this property is true, the virtual machine appends new data to the file; otherwise, it replaces the existing contents of the file before writing new data to it.

## See Also

### Getting the file details

var url: URL

The URL of a file on the local file system.


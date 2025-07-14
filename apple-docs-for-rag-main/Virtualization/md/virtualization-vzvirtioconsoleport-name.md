

- Virtualization
- VZVirtioConsolePort
-  name 

Instance Property

# name

The name of the port.

macOS 13.0+

``` source
var name: String? { get }
```

## Discussion

This property can’t change while the VM is running. A null value indicates a name isn’t set.

## See Also

### Configuring the port

var attachment: VZSerialPortAttachment?

An array of serial port attachments.


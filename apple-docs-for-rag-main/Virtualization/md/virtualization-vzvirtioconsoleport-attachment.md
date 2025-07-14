

- Virtualization
- VZVirtioConsolePort
-  attachment 

Instance Property

# attachment

An array of serial port attachments.

macOS 13.0+

``` source
var attachment: VZSerialPortAttachment? { get set }
```

## Discussion

This property may change at any time while the VM is running.

## See Also

### Configuring the port

var name: String?

The name of the port.


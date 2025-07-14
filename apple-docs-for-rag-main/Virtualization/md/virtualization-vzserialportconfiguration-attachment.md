

- Virtualization
- VZSerialPortConfiguration
-  attachment 

Instance Property

# attachment

The object that defines how the configuration of the virtual machine’s serial port interfaces.

macOS 11.0+

``` source
var attachment: VZSerialPortAttachment? { get set }
```

## Discussion

Assign an appropriate attachment object to this property, such as a VZFileHandleSerialPortAttachment or VZFileSerialPortAttachment object. When configuring the serial ports, the virtual machine uses the attachment to set up the serial port communications.


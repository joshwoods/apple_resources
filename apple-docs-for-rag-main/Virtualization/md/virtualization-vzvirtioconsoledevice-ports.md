

- Virtualization
- VZVirtioConsoleDevice
-  ports 

Instance Property

# ports

The array of console ports that a specific device uses.

macOS 13.0+

``` source
var ports: VZVirtioConsolePortArray { get }
```

## See Also

### Configuring the console

var delegate: (any VZVirtioConsoleDeviceDelegate)?

The delegate object for the console device.

protocol VZVirtioConsoleDeviceDelegate

Optional methods that you use to respond when a console port opens or closes in the virtual machine.


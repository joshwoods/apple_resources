

- Virtualization
- VZVirtioConsoleDevice
-  delegate 

Instance Property

# delegate

The delegate object for the console device.

macOS 13.0+

``` source
weak var delegate: (any VZVirtioConsoleDeviceDelegate)? { get set }
```

## See Also

### Configuring the console

var ports: VZVirtioConsolePortArray

The array of console ports that a specific device uses.

protocol VZVirtioConsoleDeviceDelegate

Optional methods that you use to respond when a console port opens or closes in the virtual machine.


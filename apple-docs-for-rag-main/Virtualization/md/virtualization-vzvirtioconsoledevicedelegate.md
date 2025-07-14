

- Virtualization
-  VZVirtioConsoleDeviceDelegate 

Protocol

# VZVirtioConsoleDeviceDelegate

Optional methods that you use to respond when a console port opens or closes in the virtual machine.

macOS 13.0+

``` source
protocol VZVirtioConsoleDeviceDelegate : NSObjectProtocol
```

## Topics

### Responding to console device changes

func consoleDevice(VZVirtioConsoleDevice, didOpen: VZVirtioConsolePort)

Tells the delegate that the framework opened a console port.

func consoleDevice(VZVirtioConsoleDevice, didClose: VZVirtioConsolePort)

Tells the delegate that the framework closed a console port.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Related Documentation

class VZVirtioConsoleDevice

A class that represents a Virtio console device in a virtual machine.

class VZVirtioConsolePort

A class that represents a Virtio console port in a VM.

### Configuring the console

var ports: VZVirtioConsolePortArray

The array of console ports that a specific device uses.

var delegate: (any VZVirtioConsoleDeviceDelegate)?

The delegate object for the console device.


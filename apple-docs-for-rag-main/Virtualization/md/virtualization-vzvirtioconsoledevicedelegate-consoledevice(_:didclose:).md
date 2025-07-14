

- Virtualization
- VZVirtioConsoleDeviceDelegate
-  consoleDevice(\_:didClose:) 

Instance Method

# consoleDevice(\_:didClose:)

Tells the delegate that the framework closed a console port.

macOS 13.0+

``` source
optional func consoleDevice(
    _ consoleDevice: VZVirtioConsoleDevice,
    didClose consolePort: VZVirtioConsolePort
)
```

## Parameters 

`consoleDevice`  

The console port’s console device.

`consolePort`  

The VZVirtioConsolePort port that the framework closed.

## Discussion

Be sure to finish processing or flushing any remaining data from the VZVirtioConsolePort attachment after closing a port, or the additional data might remain on the serial port.

## See Also

### Responding to console device changes

func consoleDevice(VZVirtioConsoleDevice, didOpen: VZVirtioConsolePort)

Tells the delegate that the framework opened a console port.


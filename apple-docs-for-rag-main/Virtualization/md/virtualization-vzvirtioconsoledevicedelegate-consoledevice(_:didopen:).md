

- Virtualization
- VZVirtioConsoleDeviceDelegate
-  consoleDevice(\_:didOpen:) 

Instance Method

# consoleDevice(\_:didOpen:)

Tells the delegate that the framework opened a console port.

macOS 13.0+

``` source
optional func consoleDevice(
    _ consoleDevice: VZVirtioConsoleDevice,
    didOpen consolePort: VZVirtioConsolePort
)
```

## Parameters 

`consoleDevice`  

The console port’s console device.

`consolePort`  

The VZVirtioConsolePort port that the framework opened.

## Discussion

Be sure to process or flush any pending data from the VZVirtioConsolePort attachment before communicating with a new virtual machine process, or additional data might remain on the serial port from the previous session.

## See Also

### Responding to console device changes

func consoleDevice(VZVirtioConsoleDevice, didClose: VZVirtioConsolePort)

Tells the delegate that the framework closed a console port.


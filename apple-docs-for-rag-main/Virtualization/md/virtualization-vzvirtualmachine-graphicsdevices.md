

- Virtualization
- VZVirtualMachine
-  graphicsDevices 

Instance Property

# graphicsDevices

The list of configured graphics devices on the virtual machine.

macOS 14.0+

``` source
var graphicsDevices: [VZGraphicsDevice] { get }
```

## Discussion

Returns an empty array if there are no graphics devices configured.

## See Also

### Related Documentation

class VZGraphicsDeviceConfiguration

The base class for a graphics device configuration.

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

### Getting the state of the VM

var state: VZVirtualMachine.State

The current execution state of the VM.

enum State

The execution states of the VM.

var canStart: Bool

A Boolean value that indicates whether you can start the VM.

var canPause: Bool

A Boolean value that indicates whether you can pause the VM.

var canResume: Bool

A Boolean value that indicates whether you can resume the VM.

var canStop: Bool

A Boolean value that indicates whether you can stop the VM.

var canRequestStop: Bool

A Boolean value that indicates whether you can ask the guest operating system to stop running.


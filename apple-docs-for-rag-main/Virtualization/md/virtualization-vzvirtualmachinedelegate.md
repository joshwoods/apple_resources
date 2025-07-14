

- Virtualization
-  VZVirtualMachineDelegate 

Protocol

# VZVirtualMachineDelegate

The methods you use to respond to changes in the state of the VM.

macOS 11.0+

``` source
protocol VZVirtualMachineDelegate : NSObjectProtocol
```

## Topics

### Stopping the VM

func guestDidStop(VZVirtualMachine)

Tells the delegate that the guest operating system stopped the VM.

func virtualMachine(VZVirtualMachine, didStopWithError: any Error)

Tells the delegate that the VM stopped because of an error.

### Responding to network device errors

func virtualMachine(VZVirtualMachine, networkDevice: VZNetworkDevice, attachmentWasDisconnectedWithError: any Error)

The method the framework calls when an error causes a VM’s network attachment to disconnect.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to a stopped VM

var delegate: (any VZVirtualMachineDelegate)?

A custom object you use to determine when the VM stops.




- Virtualization
- VZVirtualMachineDelegate
-  guestDidStop(\_:) 

Instance Method

# guestDidStop(\_:)

Tells the delegate that the guest operating system stopped the VM.

macOS 11.0+

``` source
optional func guestDidStop(_ virtualMachine: VZVirtualMachine)
```

## Parameters 

`virtualMachine`  

The VM that called the delegate method.

## See Also

### Stopping the VM

func virtualMachine(VZVirtualMachine, didStopWithError: any Error)

Tells the delegate that the VM stopped because of an error.


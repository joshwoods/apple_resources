

- Virtualization
- VZVirtualMachineDelegate
-  virtualMachine(\_:didStopWithError:) 

Instance Method

# virtualMachine(\_:didStopWithError:)

Tells the delegate that the VM stopped because of an error.

macOS 11.0+

``` source
optional func virtualMachine(
    _ virtualMachine: VZVirtualMachine,
    didStopWithError error: any Error
)
```

## Parameters 

`virtualMachine`  

The VM that called the delegate method.

`error`  

The error.

## See Also

### Stopping the VM

func guestDidStop(VZVirtualMachine)

Tells the delegate that the guest operating system stopped the VM.


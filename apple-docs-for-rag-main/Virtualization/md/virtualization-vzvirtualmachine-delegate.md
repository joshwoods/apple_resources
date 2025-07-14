

- Virtualization
- VZVirtualMachine
-  delegate 

Instance Property

# delegate

A custom object you use to determine when the VM stops.

macOS 11.0+

``` source
weak var delegate: (any VZVirtualMachineDelegate)? { get set }
```

## See Also

### Responding to a stopped VM

protocol VZVirtualMachineDelegate

The methods you use to respond to changes in the state of the VM.


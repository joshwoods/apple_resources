

- Virtualization
- VZVirtualMachine
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the system supports virtualization.

macOS 11.0+

``` source
class var isSupported: Bool { get }
```

## Discussion

If virtualization is unavailable on the current device, no configuration is valid. If you want to know more about why virtualization is unavailable, call the validate() method of VZVirtualMachineConfiguration and examine the returned error object.

## See Also

### Creating the VM

convenience init(configuration: VZVirtualMachineConfiguration)

Creates the VM and configures it with the specified data.

init(configuration: VZVirtualMachineConfiguration, queue: dispatch_queue_t)

Creates and configures the VM with the specified data and dispatch queue.


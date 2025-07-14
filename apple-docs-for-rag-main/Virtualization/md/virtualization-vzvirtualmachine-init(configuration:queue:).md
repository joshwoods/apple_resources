

- Virtualization
- VZVirtualMachine
-  init(configuration:queue:) 

Initializer

# init(configuration:queue:)

Creates and configures the VM with the specified data and dispatch queue.

macOS 11.0+

``` source
init(
    configuration: VZVirtualMachineConfiguration,
    queue: dispatch_queue_t
)
```

## Parameters 

`configuration`  

The configuration of the VM. The configuration must be valid, and you can verify that it’s valid by calling its validate() method. The VM stores a copy of the configuration.

`queue`  

The serial dispatch queue for the VM. You must perform all VM-related operations on the specified queue, and the VM executes callbacks and delegate methods on the queue. If the queue isn’t serial, the behavior isn’t defined.

## Return Value

An initialized VM object.

## See Also

### Creating the VM

convenience init(configuration: VZVirtualMachineConfiguration)

Creates the VM and configures it with the specified data.

class var isSupported: Bool

A Boolean value that indicates whether the system supports virtualization.


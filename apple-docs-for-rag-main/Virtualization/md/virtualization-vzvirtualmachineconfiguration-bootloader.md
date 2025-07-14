

- Virtualization
- VZVirtualMachineConfiguration
-  bootLoader 

Instance Property

# bootLoader

The guest system to boot when the VM starts.

macOS 11.0+

``` source
var bootLoader: VZBootLoader? { get set }
```

## Discussion

Assign the boot loader object that contains information about how to load your guest operating system. For example, to configure your VM with a Linux operating system, assign a VZLinuxBootLoader object.


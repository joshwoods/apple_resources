

- Virtualization
- VZVirtualMachineConfiguration
-  cpuCount 

Instance Property

# cpuCount

The number of CPUs you make available to the guest operating system.

macOS 11.0+

``` source
var cpuCount: Int { get set }
```

## Discussion

The value of this property must be greater than or equal to the value in minimumAllowedCPUCount, and less than or equal to the value in maximumAllowedCPUCount. The system uses the number of physical CPUs on the current system to determine a default value.

## See Also

### Setting the number of CPUs

class var minimumAllowedCPUCount: Int

The minimum number of CPUs you may configure for the VM.

class var maximumAllowedCPUCount: Int

The maximum number of CPUs you may configure for the VM.


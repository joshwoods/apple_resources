

- Virtualization
- VZVirtualMachineConfiguration
-  maximumAllowedCPUCount 

Type Property

# maximumAllowedCPUCount

The maximum number of CPUs you may configure for the VM.

macOS

``` source
class var maximumAllowedCPUCount: Int { get }
```

## Discussion

The value in the cpuCount property must be less than or equal to the value in this property.

## See Also

### Setting the number of CPUs

var cpuCount: Int

The number of CPUs you make available to the guest operating system.

class var minimumAllowedCPUCount: Int

The minimum number of CPUs you may configure for the VM.


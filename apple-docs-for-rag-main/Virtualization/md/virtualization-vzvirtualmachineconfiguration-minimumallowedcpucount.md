

- Virtualization
- VZVirtualMachineConfiguration
-  minimumAllowedCPUCount 

Type Property

# minimumAllowedCPUCount

The minimum number of CPUs you may configure for the VM.

macOS

``` source
class var minimumAllowedCPUCount: Int { get }
```

## Discussion

The value in the cpuCount property must be greater than or equal to the value in this property.

## See Also

### Setting the number of CPUs

var cpuCount: Int

The number of CPUs you make available to the guest operating system.

class var maximumAllowedCPUCount: Int

The maximum number of CPUs you may configure for the VM.


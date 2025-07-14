

- Virtualization
- VZMacOSConfigurationRequirements
-  minimumSupportedCPUCount 

Instance Property

# minimumSupportedCPUCount

The minimum supported number of CPUs for this configuration.

macOS 12.0+

``` source
var minimumSupportedCPUCount: Int { get }
```

## Discussion

This property specifies the minimum number of CPUs required by the associated macOS configuration.

You associate a VZMacOSConfigurationRequirements with a specific VZMacOSRestoreImage object, which results in a specific macOS configuration.

Installing or running the associated configuration of macOS on a virtual machine with fewer than the specified number of CPUs results in undefined behavior.

## See Also

### Configuration Requirements

var hardwareModel: VZMacHardwareModel

The hardware model for this configuration.

var minimumSupportedMemorySize: UInt64

The minimum supported memory size for this configuration.


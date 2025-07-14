

- Virtualization
- VZMacOSConfigurationRequirements
-  minimumSupportedMemorySize 

Instance Property

# minimumSupportedMemorySize

The minimum supported memory size for this configuration.

macOS 12.0+

``` source
var minimumSupportedMemorySize: UInt64 { get }
```

## Discussion

This property specifies the minimum amount of memory required by the associated macOS configuration.

You associate a VZMacOSConfigurationRequirements with a specific VZMacOSRestoreImage object, which results in a specific macOS configuration.

Installing or running the associated configuration of macOS on a VM with less than this amount of memory results in undefined behavior.

## See Also

### Configuration Requirements

var hardwareModel: VZMacHardwareModel

The hardware model for this configuration.

var minimumSupportedCPUCount: Int

The minimum supported number of CPUs for this configuration.


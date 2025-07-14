

- Virtualization
- VZMacOSConfigurationRequirements
-  hardwareModel 

Instance Property

# hardwareModel

The hardware model for this configuration.

macOS 12.0+

``` source
@NSCopying
var hardwareModel: VZMacHardwareModel { get }
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

Use a hardware model to configure a new VM that meets a set of specific requirements.

After creating the hardware model, use `VZMacPlatformConfiguration` hardwareModel to configure the Mac platform, and init(creatingStorageAt:hardwareModel:options:) to create its auxiliary storage.

## See Also

### Related Documentation

class VZMacPlatformConfiguration

The platform configuration for booting macOS on Apple silicon.

class VZMacAuxiliaryStorage

An object that contains information the boot loader needs for booting macOS as a guest operating system.

### Configuration Requirements

var minimumSupportedCPUCount: Int

The minimum supported number of CPUs for this configuration.

var minimumSupportedMemorySize: UInt64

The minimum supported memory size for this configuration.


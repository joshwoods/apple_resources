

- Virtualization
- VZMacPlatformConfiguration
-  hardwareModel 

Instance Property

# hardwareModel

The Mac hardware model.

macOS 12.0+

``` source
@NSCopying
var hardwareModel: VZMacHardwareModel { get set }
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

When creating a VM, the hardwareModel depends on the restore image that you use to install macOS.

To choose the hardware model, start from `VZMacOSRestoreImage`.mostFeaturefulSupportedConfiguration to get a supported configuration, then use its `VZMacOSConfigurationRequirements`.hardwareModel property to get the hardware model.

## See Also

### Getting platform properties

var auxiliaryStorage: VZMacAuxiliaryStorage?

The Mac auxiliary storage.

var machineIdentifier: VZMacMachineIdentifier

The Mac machine identifier.


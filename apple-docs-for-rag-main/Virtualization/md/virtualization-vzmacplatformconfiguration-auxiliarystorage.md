

- Virtualization
- VZMacPlatformConfiguration
-  auxiliaryStorage 

Instance Property

# auxiliaryStorage

The Mac auxiliary storage.

macOS 12.0+

``` source
var auxiliaryStorage: VZMacAuxiliaryStorage? { get set }
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

When creating a VM, the hardware model of the `auxiliaryStorage` must match the hardware model of the `hardwareModel` property. Defaults to `nil`, but you must set a value for a configuration to be valid.

## See Also

### Getting platform properties

var hardwareModel: VZMacHardwareModel

The Mac hardware model.

var machineIdentifier: VZMacMachineIdentifier

The Mac machine identifier.


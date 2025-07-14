

- Virtualization
- VZMacPlatformConfiguration
-  machineIdentifier 

Instance Property

# machineIdentifier

The Mac machine identifier.

macOS 12.0+

``` source
@NSCopying
var machineIdentifier: VZMacMachineIdentifier { get set }
```

## Discussion

This value uniquely identifies an instance of a VM. Running two VMs concurrently with the same identifier results in undefined behavior in the guest operating system.

## See Also

### Getting platform properties

var auxiliaryStorage: VZMacAuxiliaryStorage?

The Mac auxiliary storage.

var hardwareModel: VZMacHardwareModel

The Mac hardware model.


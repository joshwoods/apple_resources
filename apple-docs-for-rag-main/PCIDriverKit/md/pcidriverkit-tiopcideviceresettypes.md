

- PCIDriverKit
-  tIOPCIDeviceResetTypes 

Enumeration

# tIOPCIDeviceResetTypes

DriverKitmacOS

``` source
typedef enum tIOPCIDeviceResetTypes : unsigned int { ... } tIOPCIDeviceResetTypes;
```

## Overview

```
        This will issue a hot reset from its upstream bridge by setting the secondary bus reset bit in the bridge's control
        register.
```

```
        specific function exists.
```

```
        specific function exists. Upon completion, the device is unusable until the caller requests reset with type
        kIOPCIDeviceResetTypeWarmResetEnable.

        This type facilitates the generation of a cold reset, i.e. by removing power before using kIOPCIDeviceResetTypeWarmResetDisable
        and re-applying it before using kIOPCIDeviceResetTypeWarmResetEnable.
```

```
        (e.g. deassert PERST#). See kIOPCIDeviceResetTypeWarmResetDisable for more details.
```

## Topics

### Enumeration Cases

kIOPCIDeviceResetTypeFunctionReset

kIOPCIDeviceResetTypeHotReset

kIOPCIDeviceResetTypeWarmReset

kIOPCIDeviceResetTypeWarmResetDisable

kIOPCIDeviceResetTypeWarmResetEnable

## See Also

### Enumerations

Anonymous

tIOPCIAccessOptions

tIOPCIDeviceResetOptions

tIOPCILinkSpeed

IOPCIBARType

IOPCILinkSpeed

IOPCIMemoryRange

IOPCISaveDeviceStateOptions

tIOPCIAccessOptions

tIOPCIDeviceResetOptions

tIOPCILinkControlASPMBits

tIOPCILinkSpeed

Interrupt Types

Interrupt types that the device supports.


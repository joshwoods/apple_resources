

- PCIDriverKit
-  tIOPCIDeviceResetOptions 

Enumeration

# tIOPCIDeviceResetOptions

DriverKitmacOS

``` source
typedef enum tIOPCIDeviceResetOptions : unsigned int { ... } tIOPCIDeviceResetOptions;
```

## Overview

```
        any attached client drivers. Devices with reset-initiated personality changes should use this option.

        This option causes the reset function to initiate the asynchronous termination process, but not block on its completion.
```

## Topics

### Enumeration Cases

kIOPCIDeviceResetOptionNone

kIOPCIDeviceResetOptionTerminate

## See Also

### Enumerations

Anonymous

tIOPCIAccessOptions

tIOPCIDeviceResetTypes

tIOPCILinkSpeed

IOPCIBARType

IOPCILinkSpeed

IOPCIMemoryRange

IOPCISaveDeviceStateOptions

tIOPCIAccessOptions

tIOPCIDeviceResetTypes

tIOPCILinkControlASPMBits

tIOPCILinkSpeed

Interrupt Types

Interrupt types that the device supports.


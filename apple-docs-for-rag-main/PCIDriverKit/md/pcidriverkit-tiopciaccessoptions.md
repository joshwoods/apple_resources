

- PCIDriverKit
-  tIOPCIAccessOptions 

Enumeration

# tIOPCIAccessOptions

DriverKitmacOS

``` source
typedef enum tIOPCIAccessOptions : unsigned int { ... } tIOPCIAccessOptions;
```

## Overview

```
        and host software is permitted to offload the access to a DMA engine in order to free the CPU for other work to
        optimize overall system performance. Use of this hint may increase the latency of the memory space accessor function.
```

## Topics

### Enumeration Cases

kIOPCIAccessLatencyTolerantHint

## See Also

### Enumerations

Anonymous

tIOPCIDeviceResetOptions

tIOPCIDeviceResetTypes

tIOPCILinkSpeed

IOPCIBARType

IOPCILinkSpeed

IOPCIMemoryRange

IOPCISaveDeviceStateOptions

tIOPCIDeviceResetOptions

tIOPCIDeviceResetTypes

tIOPCILinkControlASPMBits

tIOPCILinkSpeed

Interrupt Types

Interrupt types that the device supports.


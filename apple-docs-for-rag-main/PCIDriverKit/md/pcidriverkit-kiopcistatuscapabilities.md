

- PCIDriverKit
-  kIOPCIStatusCapabilities 

Enumeration Case

# kIOPCIStatusCapabilities

The bit that indicates the presence of an extended capability list item.

DriverKitmacOS

``` source
kIOPCIStatusCapabilities
```

## See Also

### Registers

kIOPCIStatusInterrupt

The bit that contains the interrupt status.

kIOPCIStatusPCI66

The bit that indicates the device is capable of 66 MHz operation.

kIOPCIStatusUDF

The bit that indicates the status of UDF support.

kIOPCIStatusFastBack2Back

The bit that indicates whether the device is capable of fast back-to-back transactions.

kIOPCIStatusTargetAbortCapable

The bit that indicates whether a function completed a posted or non-posted request as a completer abort error.

kIOPCIStatusTargetAbortActive

The bit that indicates whether a requester received a completion with a completer abort completion status.

kIOPCIStatusMasterAbortActive

The bit that indicates whether a requester received a completion with an unsupported request completion status

kIOPCIStatusSERRActive

The bit that indicates whether a function sent a fatal or nonfatal error message and set the SERR enable bit in the command register.

kIOPCIStatusParityErrActive

The bit that indicates whether a function received a poisoned transaction-layer packet.

kIOPCIStatusDevSel0

The DEVSEL timing status is set to 0.

kIOPCIStatusDevSel1

The DEVSEL timing status is set to 1.

kIOPCIStatusDevSel2

The DEVSEL timing status is set to 2.

kIOPCIStatusDevSel3

The DEVSEL timing status is set to 3.


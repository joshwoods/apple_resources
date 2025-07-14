

- SCSIControllerDriverKit
-  kIOServicePowerCapabilityPause 

Macro

# kIOServicePowerCapabilityPause

A PCIe-specific power state for halting transactions while reallocating resources.

DriverKit

``` source
#define kIOServicePowerCapabilityPause
```

## Discussion

IOUserSCSIParallelInterfaceController supports this power state, in addition to the kIOServicePowerCapabilityOn and kIOServicePowerCapabilityOff power states defined in the base DriverKit framework. Implement the SetPowerState method in your service object and use it to put your driver in a safe state for any of these power states.


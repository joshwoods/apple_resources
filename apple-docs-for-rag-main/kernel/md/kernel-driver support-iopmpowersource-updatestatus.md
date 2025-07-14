

- Kernel
- Driver Support
- IOPMPowerSource
-  updateStatus 

# updateStatus

Must be called by physical battery controller when battery state has changed significantly.

``` source
virtual void updateStatus(
 void); 
```

## Overview

The system will not poll this object for battery updates. Rather \\ the battery's controller must call updateStatus() every time state changes \\ and the settings will be relayed to higher levels of power management. \\ The subclassing driver should override this only if the driver needs to add \\ new settings to the base class.

## See Also

### Miscellaneous

powerSource

Creates a new IOPMPowerSource nub. Must be attached to IORegistry, and registered by provider.

setPSProperty


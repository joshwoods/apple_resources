

- Kernel
- Driver Support
- IOPMPowerSource
-  setPSProperty 

# setPSProperty

``` source
void setPSProperty(
 const OSSymbol *,
 OSObject *); 
```

## Overview

All of these methods funnel through the generic accessor method setPSProperty. Caller can pass in any arbitrary OSSymbol key, and that value will be stored in the PM settings dictionary, and relayed onto the IORegistry at update time.

## See Also

### Miscellaneous

powerSource

Creates a new IOPMPowerSource nub. Must be attached to IORegistry, and registered by provider.

updateStatus

Must be called by physical battery controller when battery state has changed significantly.


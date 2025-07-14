

- Kernel
- Driver Support
- IOPowerConnection
-  childHasRequestedPower 

# childHasRequestedPower

Return the flag that says whether the child has called requestPowerDomainState.

``` source
bool childHasRequestedPower (
 void ); 
```

## Overview

Called by the PCI Aux Power Supply Driver to see if a device driver is power managed.

## See Also

### Miscellaneous

getAwaitingAck

Returns the awaitingAck variable.

getDesiredDomainState

Returns the desiredDomainState variable.

getPreventIdleSleepFlag

Returns the preventIdleSleepFlag variable.

getPreventSystemSleepFlag

Returns the preventSystemSleepFlag variable.

getReadyFlag

Returns the readyFlag variable.

parentCurrentPowerFlags

Returns the currentPowerFlags variable.

parentKnowsState

Returns the stateKnown variable.

setAwaitingAck

Sets the awaitingAck variable.

setChildHasRequestedPower

Set the flag that says that the child has called requestPowerDomainState.

setDesiredDomainState

Sets the desiredDomainState variable.

setParentCurrentPowerFlags

Sets the currentPowerFlags variable.

setParentKnowsState

Sets the stateKnown variable.

setPreventIdleSleepFlag

Sets the preventIdleSleepFlag variable.

setPreventSystemSleepFlag

Sets the preventSystemSleepFlag variable.

setReadyFlag

Sets the readyFlag variable.


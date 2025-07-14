

- Kernel
- Driver Support
- IOPowerConnection
-  setPreventSystemSleepFlag 

# setPreventSystemSleepFlag

Sets the preventSystemSleepFlag variable.

``` source
void setPreventSystemSleepFlag (
 unsigned long ); 
```

## Overview

Called by the parent.

## See Also

### Miscellaneous

childHasRequestedPower

Return the flag that says whether the child has called requestPowerDomainState.

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

setReadyFlag

Sets the readyFlag variable.


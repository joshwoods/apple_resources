

- Kernel
- Hardware Families
- Audio
- IOAudioDevice
-  pendingPowerState 

# pendingPowerState

``` source
IOAudioDevicePowerState pendingPowerState;
```

## Overview

If a power state change is in progress, this represents the pending power state. All other times this is the same as the currentPowerState.

## See Also

### Instance Variables

workLoop

timerEventSource

timerEvents

The set of timer events in use by the device.

numRunningAudioEngines

minimumInterval

familyManagePower

duringStartup

currentPowerState

commandGate

audioPorts

audioEngines

asyncPowerStateChangeInProgress


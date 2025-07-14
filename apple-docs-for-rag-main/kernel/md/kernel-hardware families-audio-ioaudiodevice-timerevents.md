

- Kernel
- Hardware Families
- Audio
- IOAudioDevice
-  timerEvents 

# timerEvents

The set of timer events in use by the device.

``` source
OSDictionary * timerEvents;
```

## Overview

The key for the dictionary is the target of the event. This means that a single target may have only a single event associated with it.

## See Also

### Instance Variables

workLoop

timerEventSource

pendingPowerState

numRunningAudioEngines

minimumInterval

familyManagePower

duringStartup

currentPowerState

commandGate

audioPorts

audioEngines

asyncPowerStateChangeInProgress


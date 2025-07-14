

- Kernel
- Hardware Families
- Audio
- IOAudioDevice
-  TimerEvent 

# TimerEvent

Generic timer event callback for IOAudioDevice timer targets

``` source
typedef void ( *TimerEvent)(
   OSObject *target,
   IOAudioDevice *audioDevice);
```

## Parameters 

`target`  

The target of the timer event - passed in when the timer event was registered

`audioDevice`  

The IOAudioDevice sending the event

## Overview

TimerEvent callback function takes two arguments; the target of the timer event and the IOAudioDevice sending the event.




- Kernel
- Kernel Enumerations
-  IOAudioDevicePowerState 

Enumeration

# IOAudioDevicePowerState

Identifies the power state of the audio device

macOS 10.1+

``` source
typedef enum _IOAudioDevicePowerState : unsigned int {
    ...
} IOAudioDevicePowerState;
```

## Overview

A newly created IOAudioDevices defaults to the idle state.

## Topics

### Constants

kIOAudioDeviceSleep

kIOAudioDeviceIdle

kIOAudioDeviceActive




- Force Feedback
-  ForceFeedbackDeviceState 

Structure

# ForceFeedbackDeviceState

Returns information about the state of a force feedback device.

Mac Catalyst 13.0+macOS 10.2+

``` source
struct ForceFeedbackDeviceState;
```

## Topics

### Instance Properties

dwLoad

A value indicating the percentage of device memory in use. A value of zero indicates that the device memory is completely available. A value of 100 indicates that the device is full

dwSize

Specifies the size of the structure in bytes. This member must be initialized before the structure is used.

dwState

Indicates various aspects of the device state.

## See Also

### Data Types

FFEffectDownloadID

Unique identification for an effect.

ForceFeedbackVersion

Used to return plugIn version information.


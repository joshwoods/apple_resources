

- AudioDriverKit
-  IOUserAudioDevice 

Class

# IOUserAudioDevice

An audio clock device object that handles the configurations for running I/O.

DriverKit 21.0+

``` source
class IOUserAudioDevice;
```

## Overview

The IOUserAudioDevice class subclasses IOUserAudioClockDevice and can contain IOUserAudioStream instances that perform I/O for the audio device.

## Topics

### Creating an Audio Device

Create

Allocates and initializes an instance of the audio device class.

init

Initializes an instance of the audio device class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

### Freeing an Audio Device

free

Frees the audio device.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

### Performing I/O

StartIO

Tells the device to start I/O.

StopIO

Tells the device to stop I/O.

IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

### Supporting Device Configuration Changes

PerformDeviceConfigurationChange

Tells the device to handle a configuration change.

AbortDeviceConfigurationChange

Tells the device to stop handling a configuration change.

### Supporting Sample Rate Changes

HandleChangeSampleRate

Tells the device the sample rate is changing.

DeviceSampleRateChanged

Updates stream formats, in response to the owning audio device changing its sample rate.

### Working with Audio Streams

AddStream

Adds an audio stream to the device.

RemoveStream

Removes an audio stream from the device.

IOUserAudioStream

An audio object that performs I/O for an audio device.

### Working with Default Device Behavior

SetCanBeDefaultInputDevice

Sets a Boolean value that indicates if this device can be the host’s default input device.

CanBeDefaultInputDevice

Returns a Boolean value that indicates if this device can be the host’s default input device.

SetCanBeDefaultOutputDevice

Sets a Boolean value that indicates if this device can be the host’s default output device.

CanBeDefaultOutputDevice

Returns a Boolean value that indicates if this device can be the host’s default output device.

SetCanBeDefaultSystemOutputDevice

Sets a Boolean value that indicates if this device can be the system’s default output device.

CanBeDefaultSystemOutputDevice

Returns a Boolean value that indicates if this device can be the system’s default output device.

### Working with Safety Offset Behvaior

SetInputSafetyOffset

Specifies the input safety offset of the device.

GetInputSafetyOffset

Returns the input safety offset of the device.

SetOutputSafetyOffset

Specifies the output safety offset of the device.

GetOutputSafetyOffset

Returns the output safety offset of the device.

### Working with Channel Layouts

SetPreferredChannelsForStereo

Sets the channel indices for the prefered stereo pair.

GetPreferredChannelsForStereo

Returns the channel indices for the prefered stereo pair.

SetPreferredInputChannelLayout

Sets the input channel layout, using an array of audio channel label values.

SetPreferredOutputChannelLayout

Sets the output channel layout, using an array of audio channel label values.

IOUserAudioChannelLabel

Constants to set the preferred channel layout on an audio device.

### Instance Methods

GetCurrentClientIOTime

SetIOOperationHandler

## Relationships

### Inherits From

- IOUserAudioClockDevice

## See Also

### Working with Audio Devices

IOUserAudioClockDevice

An audio clock device object, used to synchronize and perform I/O.


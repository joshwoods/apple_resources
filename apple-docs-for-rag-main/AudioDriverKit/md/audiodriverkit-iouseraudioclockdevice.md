

- AudioDriverKit
-  IOUserAudioClockDevice 

Class

# IOUserAudioClockDevice

An audio clock device object, used to synchronize and perform I/O.

DriverKit 21.0+

``` source
class IOUserAudioClockDevice;
```

## Topics

### Creating a Clock Device

Create

Allocates and initializes an instance of the audio clock device class.

init

Initializes an instance of the audio clock device class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

### Freeing a Clock Device

free

Frees the clock device.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

### Performing I/O

StartIO

Tells the clock device to start I/O.

StopIO

Tells the clock device to stop I/O.

IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

### Supporting Device Configuration Changes

PerformDeviceConfigurationChange

Tells the clock device to handle a configuration change.

AbortDeviceConfigurationChange

Tells the clock device to stop handling a configuration change.

### Supporting Sample Rate Changes

HandleChangeSampleRate

Tells the clock device the sample rate is changing.

### Identifying the Clock Device

GetUID

Gets the unique identifier of the clock device.

### Working with Clock Domain

SetClockDomain

Sets the clock domain value of the clock device.

GetClockDomain

Gets the clock domain value of the clock device.

### Working with Sample Rates

SetSampleRate

Sets the sample rate for the clock device.

GetSampleRate

Gets the sample rate of the clock device.

SetAvailableSampleRates

Sets the available sample rates for the clock device.

GetAvailableSampleRates

Gets the available sample rates of the clock device.

GetNumberAvailableSampleRates

Gets the number of available sample rates of the clock device.

### Working with Timing and Latency

GetSupportsPrewarming

Returns a Boolean value that indicates clock device’s support for prewarming.

SetZeroTimeStampPeriod

Sets the zero time stamp of the clock device.

GetZeroTimestampPeriod

Gets the zero time stamp of the clock device.

SetOutputLatency

Sets the output latency of the clock device.

GetOutputLatency

Gets the output latency of the clock device.

SetInputLatency

Sets the input latency of the clock device.

GetInputLatency

Get the input latency of the clock device.

### Working with Clock Device State

GetDeviceIsRunning

Gets a Boolean value that indicates whether the device is running.

SetDeviceIsAlive

Sets a Boolean value to represent whether the device is alive.

GetDeviceIsAlive

Gets a Boolean value that represents whether the device is alive.

SetIsHidden

Sets a Boolean value to indicate whether the device is hidden.

GetIsHidden

Gets a Boolean value that indicates whether the device is hidden.

### Working with Clock Device Behavior

SetClockAlgorithm

Sets the clock algorithm of the clock device.

GetClockAlgorithm

Gets the clock algorithm of the clock device.

IOUserAudioClockAlgorithm

Values that describe clock-smoothing algorithms.

SetClockIsStable

Sets a Boolean value to represent the clock’s stability.

GetClockIsStable

Gets a Boolean value that represents the clock’s stability.

### Working with Transport Type

SetTransportType

Sets the transport type of the clock device.

GetTransportType

Gets the transport type of the clock device.

IOUserAudioTransportType

The type of transport to deliver audio.

### Communicating with the Host

RequestDeviceConfigurationChange

Instructs the host to initiate a configuration change operation.

### Managing Audio Controls

AddControl

Adds a control to the clock device.

RemoveControl

Removes a control from the clock device.

IOUserAudioControl

The base class for audio control objects.

### Accessing Timestamps

UpdateCurrentZeroTimestamp

Updates the current timestamp value.

GetCurrentZeroTimestamp

Gets the current zero timestamp value.

### Accessing Client Status Information

GetCurrentClientSampleTime

Gets the current sample time in the ring buffer that the client has written to or read from.

### Instance Methods

GetDeviceTransportState

## Relationships

### Inherits From

- IOUserAudioObject

### Inherited By

- IOUserAudioDevice

## See Also

### Working with Audio Devices

IOUserAudioDevice

An audio clock device object that handles the configurations for running I/O.


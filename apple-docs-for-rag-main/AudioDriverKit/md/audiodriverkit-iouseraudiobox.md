

- AudioDriverKit
-  IOUserAudioBox 

Class

# IOUserAudioBox

A container for other audio objects, typically audio devices and audio clock devices.

DriverKit 21.0+

``` source
class IOUserAudioBox;
```

## Overview

Along with containing other audio objects, IOUserAudioBox publishes identifying information about itself and allows you to enable or disable the box. When disabled, the box’s contents aren’t available.

## Topics

### Creating an Audio Box

Create

Allocates and initializes an instance of the audio box class.

init

Initializes an instance of the audio box class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

### Freeing an Audio Box

free

Frees the audio box.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

### Identifying the Box

GetUID

Returns the UID of the audio box.

### Managing Box Contents

AddDevice

Adds an audio device to the audio box.

RemoveDevice

Removes an audio device from the audio box.

IOUserAudioDevice

An audio clock device object that handles the configurations for running I/O.

AddClockDevice

Adds an audio clock device to the audio box.

RemoveClockDevice

Adds an audio clock device to the audio box.

IOUserAudioClockDevice

An audio clock device object, used to synchronize and perform I/O.

### Managing Protection State

SetIsProtected

Sets a Boolean value that indicates if the box requires authentication before use.

IsProtected

Returns a Boolean value that indicates if the box requires authentication before use.

### Managing Acquirability

HandleChangeAcquireBox

Informs the box of a change to its acquisition state.

SetIsAcquired

Set the box’s acquisition state.

IsAcquired

Returns a Boolean value that indicates the box’s acquisition state.

SetIsAcquirable

Set the box’s acquirability state.

IsAcquirable

Returns a Boolean value that indicates the box’s acquirabilty state.

SetAcquisitionFailure

Sets the error code to return when box acquisition fails.

GetAcquisitionFailure

Returns the error code for use when box acquisition fails.

### Determining Media Support

SetHasAudio

Sets a Boolean value that indicates the box’s audio support.

HasAudio

Returns a Boolean value that indicates the box’s audio support.

SetHasVideo

Sets a Boolean value that indicates the box’s video support.

HasVideo

Returns a Boolean value that indicates the box’s video support.

SetHasMIDI

Sets a Boolean value that indicates the box’s MIDI support.

HasMIDI

Returns a Boolean value that indicates the box’s MIDI support.

### Working with Transport Types

SetTransportType

Sets the box’s transport type.

GetTransportType

Returns the box’s transport type.

IOUserAudioTransportType

The type of transport to deliver audio.

## Relationships

### Inherits From

- IOUserAudioObject


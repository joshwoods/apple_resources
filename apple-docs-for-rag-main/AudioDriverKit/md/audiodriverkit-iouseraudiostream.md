

- AudioDriverKit
-  IOUserAudioStream 

Class

# IOUserAudioStream

An audio object that performs I/O for an audio device.

DriverKit 21.0+

``` source
class IOUserAudioStream;
```

## Overview

IOUserAudioStream allocates memory descriptors that the host uses for running I/O. An IOUserAudioDevice uses an IOUserAudioStream instance to perform I/O. Changes to the device that owns a stream may update formats on the underlying stream, which you handle by overriding HandleChangeCurrentStreamFormat and HandleChangeStreamIsActive.

## Topics

### Creating an Audio Stream

Create

Allocates and initializes an instance of the audio stream class.

init

Initializes an instance of the audio stream class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

### Freeing an Audio Stream

free

Frees the audio stream.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

### Performing I/O

StartIO

Tells the stream to start I/O.

StopIO

Tells the stream to stop I/O.

IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

### Working with Stream Formats

SetCurrentStreamFormat

Sets the current stream format to a given audio stream basic description.

GetCurrentStreamFormat

Returns the current stream format, as an audio stream basic description.

SetAvailableStreamFormats

Sets the available stream formats to an array of audio stream basic descriptions.

GetAvailableStreamFormats

Returns the available stream formats as an array of audio stream basic descriptions.

GetNumberAvailableStreamFormats

Returns the number of available stream formats.

IOUserAudioStreamBasicDescription

A structure that encapsulates all of the information for describing the basic format properties of a stream of audio data.

GetStreamDirection

Gets the direction of the stream: input or output.

IOUserAudioStreamDirection

A type representing the direction of audio flow.

SetStreamIsActive

Sets a Boolean value that indicates whether the stream is active and doing I/O.

GetStreamIsActive

Gets a value that indicates whether the stream is active and doing I/O.

### Working with Stream Terminals

SetTerminalType

Sets the terminal type of the stream.

GetTerminalType

Gets the terminal type of the stream.

IOUserAudioStreamTerminalType

Constants that describe the terminal type of an audio stream.

### Working with Memory Descriptors

GetIOMemoryDescriptor

Gets the memory descriptor the stream uses for I/O.

SetIOMemoryDescriptor

Sets the memory descriptor the stream uses for I/O.

### Managing Stream Changes

HandleChangeCurrentStreamFormat

Tells the stream the format is changing.

HandleChangeStreamIsActive

Tells the stream the activity state is changing.

DeviceSampleRateChanged

Updates stream formats, in response to the owning audio device changing its sample rate.

### Instance Methods

GetLatency

GetStartingChannel

SetLatency

SetStartingChannel

## Relationships

### Inherits From

- IOUserAudioObject


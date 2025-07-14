

- AVFoundation
-  AVCaptureAudioChannel 

Class

# AVCaptureAudioChannel

An object that monitors average and peak power levels for an audio channel in a capture connection.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
class AVCaptureAudioChannel
```

## Overview

You don’t create instances of this class directly. Instead, an AVCaptureConnection object that connects an audio input to an audio output provides an array of AVCaptureAudioChannel objects, one for each channel of audio available. You can poll for audio levels by iterating through these audio channel objects.

## Topics

### Configuring a Channel

var isEnabled: Bool

A Boolean value that indicates whether the channel is in an enabled state.

var volume: Float

The current volume (gain) of the channel.

### Accessing Power Levels

var averagePowerLevel: Float

The instantaneous average power level in decibels.

var peakHoldLevel: Float

The peak hold power level in decibels.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Connecting Inputs and Outputs

var connections: [AVCaptureConnection]

The connections between inputs and outputs that a capture session contains.

func addConnection(AVCaptureConnection)

Adds a connection to the capture session.

func canAddConnection(AVCaptureConnection) -> Bool

Determines whether a you can add a connection to a capture session.

func addInputWithNoConnections(AVCaptureInput)

Adds a capture input to a session without forming any connections.

func addOutputWithNoConnections(AVCaptureOutput)

Adds a capture output to the session without forming any connections.

func removeConnection(AVCaptureConnection)

Removes a capture connection from the session.


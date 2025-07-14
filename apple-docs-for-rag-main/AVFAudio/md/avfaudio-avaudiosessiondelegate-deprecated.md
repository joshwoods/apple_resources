

- AVFAudio
-  AVAudioSessionDelegate Deprecated

Protocol

# AVAudioSessionDelegate

A protocol that defines responses to changes in state for the audio session.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
protocol AVAudioSessionDelegate : NSObjectProtocol
```

Deprecated

The use of this protocol is deprecated in iOS 6 and later. Instead, you should use the notifications declared in AVAudioSession.

## Overview

The delegate of an `AVAudioSession` object must adopt the `AVAudioSessionDelegate` protocol. The methods in this protocol are optional. They allow a delegate to respond to the following sorts of changes in state:

- Changes to the availability of audio input

- Audio session interruption, or end of audio session interruption

An `AVAudioSession` delegate can respond to interruptions at the audio session level. You can use this interface along with any iOS audio technology. For example, your `AVAudioSession` delegate can handle interruptions for OpenAL and audio unit playback.

When using the AVFoundation framework for recording or playback, you can also respond to interruptions at the individual recorder or player level. To do this, create audio recorder or audio player delegates using the protocols described in AVAudioRecorderDelegate and AVAudioPlayerDelegate.

## Topics

### Delegate Methods

func beginInterruption()

Called after your audio session is interrupted.

func endInterruption()

Called after your audio session interruption ends.

func endInterruption(withFlags: Int)

Called after your audio session interruption ends, with flags indicating the state of the audio session.

func inputIsAvailableChanged(Bool)

Called after the availability of audio input changes on a device.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to audio session changes

var delegate: (any AVAudioSessionDelegate)?

The delegate object for the audio session.

Deprecated


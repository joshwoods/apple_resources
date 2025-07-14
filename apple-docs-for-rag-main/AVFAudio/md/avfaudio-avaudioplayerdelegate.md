

- AVFAudio
-  AVAudioPlayerDelegate 

Protocol

# AVAudioPlayerDelegate

A protocol that defines the methods to respond to audio playback events and decoding errors.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS 3.0+

``` source
protocol AVAudioPlayerDelegate : NSObjectProtocol
```

## Overview

All of the methods in this protocol are optional.

## Topics

### Responding to Playback Completion

func audioPlayerDidFinishPlaying(AVAudioPlayer, successfully: Bool)

Tells the delegate when the audio finishes playing.

### Responding to Audio Decoding Errors

func audioPlayerDecodeErrorDidOccur(AVAudioPlayer, error: (any Error)?)

Tells the delegate when an audio player encounters a decoding error during playback.

### Responding to Audio Interruptions

func audioPlayerBeginInterruption(AVAudioPlayer)

Tells the delegate when the system interrupts the audio player’s playback.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer)

Tells the delegate when the audio session interruption ends.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer, withOptions: Int)

Tells the delegate when the audio session interruption ends with options.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer, withFlags: Int)

Tells the delegate when the audio session interruption ends with flags.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to player events

var delegate: (any AVAudioPlayerDelegate)?

The delegate object for the audio player.


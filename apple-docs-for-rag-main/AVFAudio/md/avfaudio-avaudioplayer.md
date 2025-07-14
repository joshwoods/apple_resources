

- AVFAudio
-  AVAudioPlayer 

Class

# AVAudioPlayer

An object that plays audio data from a file or buffer.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class AVAudioPlayer
```

## Overview

Use an audio player to:

- Play audio of any duration from a file or buffer

- Control the volume, panning, rate, and looping behavior of the played audio

- Access playback-level metering data

- Play multiple sounds simultaneously by synchronizing the playback of multiple players

For more information about preparing your app to play audio, see Configuring your app for media playback.

Important

For more advanced playback capabilities, like playing streaming or positional audio, use AVAudioEngine instead.

## Topics

### Creating an audio player

init(contentsOf: URL) throws

Creates a player to play audio from a file.

init(contentsOf: URL, fileTypeHint: String?) throws

Creates a player to play audio from a file of a particular type.

init(data: Data) throws

Creates a player to play in-memory audio data.

init(data: Data, fileTypeHint: String?) throws

Creates a player to play in-memory audio data of a particular type.

### Controlling playback

func prepareToPlay() -> Bool

Prepares the player for audio playback.

func play() -> Bool

Plays audio asynchronously.

func play(atTime: TimeInterval) -> Bool

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

func pause()

Pauses audio playback.

func stop()

Stops playback and undoes the setup the system requires for playback.

var isPlaying: Bool

A Boolean value that indicates whether the player is currently playing audio.

### Configuring playback settings

var volume: Float

The audio player’s volume relative to other audio output.

func setVolume(Float, fadeDuration: TimeInterval)

Changes the audio player’s volume over a duration of time.

var pan: Float

The audio player’s stereo pan position.

var enableRate: Bool

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

var rate: Float

The audio player’s playback rate.

var numberOfLoops: Int

The number of times the audio repeats playback.

### Accessing player timing

var currentTime: TimeInterval

The current playback time, in seconds, within the audio timeline.

var duration: TimeInterval

The total duration, in seconds, of the player’s audio.

### Managing audio channels

var numberOfChannels: Int

The number of audio channels in the player’s audio.

var channelAssignments: [AVAudioSessionChannelDescription]?

An array of channel descriptions for the audio player.

### Managing audio-level metering

var isMeteringEnabled: Bool

A Boolean value that indicates whether the player is able to generate audio-level metering data.

func updateMeters()

Refreshes the average and peak power values for all channels of an audio player.

func averagePower(forChannel: Int) -> Float

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

func peakPower(forChannel: Int) -> Float

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

### Responding to player events

var delegate: (any AVAudioPlayerDelegate)?

The delegate object for the audio player.

protocol AVAudioPlayerDelegate

A protocol that defines the methods to respond to audio playback events and decoding errors.

### Inspecting the audio data

var url: URL?

The URL of the audio file.

var data: Data?

The audio data associated with the player.

var format: AVAudioFormat

The format of the player’s audio data.

var settings: [String : Any]

A dictionary that provides information about the player’s audio data.

### Accessing device information

var currentDevice: String?

The unique identifier of the current audio player.

var deviceCurrentTime: TimeInterval

The time value, in seconds, of the audio output device’s clock.

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

### Basic playback and recording

class AVAudioRecorder

An object that records audio data to a file.

class AVMIDIPlayer

An object that plays MIDI data through a system sound module.


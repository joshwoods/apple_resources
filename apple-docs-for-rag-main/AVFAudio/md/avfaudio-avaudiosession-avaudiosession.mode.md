

- AVFAudio
- AVAudioSession
-  AVAudioSession.Mode 

Structure

# AVAudioSession.Mode

Audio session mode identifiers.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct Mode
```

## Overview

While categories set the base behaviors for your app, you use modes to assign specialized behavior to an audio session category.

Important

Specifying a mode that the audio session category doesn’t support, such as setting the gameChat mode for the multiRoute category, results in the audio session using the default mode behavior.

## Topics

### Creating a Mode

init(rawValue: String)

Creates a new instance with the raw value you specify.

### Getting Standard Session Modes

static let `default`: AVAudioSession.Mode

The default audio session mode.

static let gameChat: AVAudioSession.Mode

A mode that the GameKit framework sets on behalf of an application that uses GameKit’s voice chat service.

static let measurement: AVAudioSession.Mode

A mode that indicates that your app is performing measurement of audio input or output.

static let moviePlayback: AVAudioSession.Mode

A mode that indicates that your app is playing back movie content.

static let spokenAudio: AVAudioSession.Mode

A mode used for continuous spoken audio to pause the audio when another app plays a short audio prompt.

static let videoChat: AVAudioSession.Mode

A mode that indicates that your app is engaging in online video conferencing.

static let videoRecording: AVAudioSession.Mode

A mode that indicates that your app is recording a movie.

static let voiceChat: AVAudioSession.Mode

A mode that indicates that your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

static let voicePrompt: AVAudioSession.Mode

A mode that indicates that your app plays audio using text-to-speech.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting mode configuration

var mode: AVAudioSession.Mode

The current audio session’s mode.

var availableModes: [AVAudioSession.Mode]

The audio session modes available on the device.


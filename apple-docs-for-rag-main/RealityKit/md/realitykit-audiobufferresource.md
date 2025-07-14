

- RealityKit
-  AudioBufferResource 

Class

# AudioBufferResource

An audio resource that you load from an AVAudioBuffer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
class AudioBufferResource
```

## Overview

Use the resource to create an AudioPlaybackController instance by calling an entity’s prepareAudio(_:) or playAudio(_:) function. The controller plays the audio from the location in space of the entity that created the controller.

## Topics

### Creating an audio buffer resource

init(buffer: AVAudioBuffer, configuration: AudioBufferResource.Configuration) throws

Creates an `AudioBufferResource` with the given `AVAudioBuffer` and configuration.

### Describing the resource

let configuration: AudioBufferResource.Configuration

The configuration for this `AudioBufferResource`.

var duration: Duration

The duration of this `AudioBufferResource`.

### Supporting types

struct Configuration

### Deprecated

init(buffer: AVAudioBuffer, inputMode: AudioResource.InputMode, shouldLoop: Bool) throws

Init an AudioBufferResource from an `AVAudioBuffer` instead of a file location. This is intended for use with `AVSpeechSynthesisVoice`.

Deprecated

var shouldLoop: Bool

Whether or not this file loops during playback. This should be set for assets that are prepared as seamless loops. A looping resource will play forever until it is explicitly told to stop.

Deprecated

### Default Implementations

Hashable Implementations

## Relationships

### Inherits From

- AudioResource

### Conforms To

- Copyable
- Equatable
- Hashable
- Resource
- Sendable

## See Also

### Audio resources

class AudioFileResource

An audio resource that you load from a file or from a URL.

class AudioFileGroupResource

An audio file group.

struct AudioLibraryComponent

A container for audio resources that you can look up by user-defined names.

class AudioResource

A playable audio resource

struct Calibration

A container for different calibration modes that can be applied for playback.

struct Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.


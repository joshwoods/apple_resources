

- RealityKit
-  AudioFileResource 

Class

# AudioFileResource

An audio resource that you load from a file or from a URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class AudioFileResource
```

## Overview

Load an audio file resource, like an audio file stored in .aiff or other format, by calling one of the load functions. Use the resource to create an AudioPlaybackController instance by calling an entity’s prepareAudio(_:) or playAudio(_:) function. The controller plays the audio from the location in space of the entity that created the controller.

## Topics

### Loading audio from a bundle

convenience init(named: String, from: String, in: Bundle?) async throws

Initializes a preconfigured AudioFileResource asynchronously from a Reality Composer Pro project with the given `name` as the the prim-path of the AudioFile, and the `scene` as the name of the USD file name.

convenience init(named: String, in: Bundle?, configuration: AudioFileResource.Configuration) async throws

Initializes an AudioFileResource asynchronously.

### Loading audio from a URL

convenience init(contentsOf: URL, withName: String?, configuration: AudioFileResource.Configuration) async throws

Initializes an AudioFileResource asynchronously.

### Describing the resource

let configuration: AudioFileResource.Configuration

The configuration of this `AudioFileResource`.

var duration: Duration

The duration of this `AudioFileResource`.

let name: String

The name of this `AudioFileResource`.

### Supporting types

struct Configuration

A container for various settings for loading an audio file resource.

enum LoadingStrategy

A container for different strategies on how to handle resources’ data before and during playback.

### Deprecated

static func load(named: String, in: Bundle?, inputMode: AudioResource.InputMode, loadingStrategy: AudioFileResource.LoadingStrategy, shouldLoop: Bool) throws -> AudioFileResource

Synchronously loads an audio resource.

Deprecated

static func loadAsync(named: String, in: Bundle?, inputMode: AudioResource.InputMode, loadingStrategy: AudioFileResource.LoadingStrategy, shouldLoop: Bool) -> LoadRequest&lt;AudioFileResource>Deprecated

static func load(contentsOf: URL, withName: String?, inputMode: AudioResource.InputMode, loadingStrategy: AudioFileResource.LoadingStrategy, shouldLoop: Bool) throws -> AudioFileResource

Synchronously loads an audio resource.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?, inputMode: AudioResource.InputMode, loadingStrategy: AudioFileResource.LoadingStrategy, shouldLoop: Bool) -> LoadRequest&lt;AudioFileResource>Deprecated

var loadingStrategy: AudioFileResource.LoadingStrategy

The resource’s memory model.

Deprecated

var shouldLoop: Bool

Whether or not this file loops during playback. This should be set for assets that are prepared as seamless loops. A looping resource will play forever until it is explicitly told to stop.

Deprecated

### Operators

static func == (AudioFileResource, AudioFileResource) -> Bool

### Type Methods

static func load(contentsOf: URL, withName: String?, configuration: AudioFileResource.Configuration) throws -> AudioFileResource

Loads an AudioFileResource synchronously.

static func load(named: String, from: String, in: Bundle?) throws -> AudioFileResource

Loads a preconfigured AudioFileResource from a Reality Composer Pro project with the given `name` as the the prim-path of the AudioFile, and the `scene` as the name of the USD file name.

static func load(named: String, in: Bundle?, configuration: AudioFileResource.Configuration) throws -> AudioFileResource

Loads an AudioFileResource synchronously.

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

class AudioFileGroupResource

An audio file group.

class AudioBufferResource

An audio resource that you load from an AVAudioBuffer.

struct AudioLibraryComponent

A container for audio resources that you can look up by user-defined names.

class AudioResource

A playable audio resource

struct Calibration

A container for different calibration modes that can be applied for playback.

struct Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.




- AVFAudio
-  AVAudioUnit 

Class

# AVAudioUnit

A subclass of the audio node class that, processes audio either in real time or nonreal time, depending on the type of the audio unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnit
```

## Topics

### Getting the Core Audio audio unit

var audioUnit: AudioUnit

The underlying Core Audio audio unit.

### Loading an audio preset file

func loadPreset(at: URL) throws

Loads an audio unit using a specified preset.

### Creating an audio unit component

class func instantiate(with: AudioComponentDescription, options: AudioComponentInstantiationOptions, completionHandler: (AVAudioUnit?, (any Error)?) -> Void)

Creates an instance of an audio unit component asynchronously and wraps it in an audio unit class.

### Getting audio unit values

var audioComponentDescription: AudioComponentDescription

The audio component description that represents the underlying Core Audio audio unit.

var manufacturerName: String

The name of the manufacturer of the audio unit.

var name: String

The name of the audio unit.

var version: Int

The version number of the audio unit.

var auAudioUnit: AUAudioUnit

The audio unit class wrapping or underlying the implementation’s audio unit.

## Relationships

### Inherits From

- AVAudioNode

### Inherited By

- AVAudioUnitEffect
- AVAudioUnitGenerator
- AVAudioUnitMIDIInstrument
- AVAudioUnitTimeEffect

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Essentials

Creating an audio unit extension

Build an extension by using an Xcode template.

Using voice processing

Add voice-processing capabilities to your app by using audio engine.


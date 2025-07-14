

- AVFAudio
- AVAudioUnit
-  auAudioUnit 

Instance Property

# auAudioUnit

The audio unit class wrapping or underlying the implementation’s audio unit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var auAudioUnit: AUAudioUnit { get }
```

## See Also

### Getting audio unit values

var audioComponentDescription: AudioComponentDescription

The audio component description that represents the underlying Core Audio audio unit.

var manufacturerName: String

The name of the manufacturer of the audio unit.

var name: String

The name of the audio unit.

var version: Int

The version number of the audio unit.


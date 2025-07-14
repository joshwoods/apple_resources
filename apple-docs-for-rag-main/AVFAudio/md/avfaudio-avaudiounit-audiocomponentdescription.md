

- AVFAudio
- AVAudioUnit
-  audioComponentDescription 

Instance Property

# audioComponentDescription

The audio component description that represents the underlying Core Audio audio unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var audioComponentDescription: AudioComponentDescription { get }
```

## See Also

### Related Documentation

var audioUnit: AudioUnit

The underlying Core Audio audio unit.

### Getting audio unit values

var manufacturerName: String

The name of the manufacturer of the audio unit.

var name: String

The name of the audio unit.

var version: Int

The version number of the audio unit.

var auAudioUnit: AUAudioUnit

The audio unit class wrapping or underlying the implementation’s audio unit.


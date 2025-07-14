

- AVFAudio
- AVAudioSession
-  preferredHardwareSampleRate Deprecated

Instance Property

# preferredHardwareSampleRate

The preferred hardware sample rate, in hertz.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var preferredHardwareSampleRate: Double { get }
```

Deprecated

Use preferredSampleRate instead.

## See Also

### Inspecting audio hardware

var currentHardwareInputNumberOfChannels: Int

The number of audio hardware input channels.

Deprecated

var currentHardwareOutputNumberOfChannels: Int

The number of audio hardware output channels.

Deprecated

var currentHardwareSampleRate: Double

The audio hardware sample rate, in hertz.

Deprecated

var inputIsAvailable: Bool

A Boolean value that indicates whether a hardware audio input path is available.

Deprecated

func setPreferredHardwareSampleRate(Double) throws

Sets the preferred hardware sample rate for input and output.

Deprecated


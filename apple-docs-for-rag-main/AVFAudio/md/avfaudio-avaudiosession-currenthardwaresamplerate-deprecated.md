

- AVFAudio
- AVAudioSession
-  currentHardwareSampleRate Deprecated

Instance Property

# currentHardwareSampleRate

The audio hardware sample rate, in hertz.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var currentHardwareSampleRate: Double { get }
```

Deprecated

Use sampleRate instead

## Discussion

Obtain the value of this property after activating your audio session. After successful activation, the value of this property doesn’t change while your session remains active.

## See Also

### Inspecting audio hardware

var currentHardwareInputNumberOfChannels: Int

The number of audio hardware input channels.

Deprecated

var currentHardwareOutputNumberOfChannels: Int

The number of audio hardware output channels.

Deprecated

var inputIsAvailable: Bool

A Boolean value that indicates whether a hardware audio input path is available.

Deprecated

var preferredHardwareSampleRate: Double

The preferred hardware sample rate, in hertz.

Deprecated

func setPreferredHardwareSampleRate(Double) throws

Sets the preferred hardware sample rate for input and output.

Deprecated


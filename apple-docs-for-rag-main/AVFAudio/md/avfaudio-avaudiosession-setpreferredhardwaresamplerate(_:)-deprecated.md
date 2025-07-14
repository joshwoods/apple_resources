

- AVFAudio
- AVAudioSession
-  setPreferredHardwareSampleRate(\_:) Deprecated

Instance Method

# setPreferredHardwareSampleRate(\_:)

Sets the preferred hardware sample rate for input and output.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func setPreferredHardwareSampleRate(_ sampleRate: Double) throws
```

Deprecated

Use setPreferredSampleRate(_:) instead.

## Parameters 

`sampleRate`  

The hardware sample rate you want to use. The available range for hardware sample rate is device dependent.

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

var preferredHardwareSampleRate: Double

The preferred hardware sample rate, in hertz.

Deprecated


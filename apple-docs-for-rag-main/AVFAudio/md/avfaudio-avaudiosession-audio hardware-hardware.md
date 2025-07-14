

- AVFAudio
- AVAudioSession
-  Audio hardware 

API Collection

# Audio hardware

Inspect and configure audio device settings including input gain, sample rate, and channel counts.

## Topics

### Configuring sample rate

var sampleRate: Double

The current audio sample rate, in hertz.

var preferredSampleRate: Double

The preferred sample rate, in hertz.

func setPreferredSampleRate(Double) throws

Sets the preferred sample rate for audio input and output.

### Setting input gain

var inputGain: Float

The gain applied to inputs associated with the session.

var isInputGainSettable: Bool

A Boolean value that indicates whether you can set the input gain.

func setInputGain(Float) throws

Changes the input gain to the specified value.

### Configuring I/O buffer duration

var ioBufferDuration: TimeInterval

The current I/O buffer duration, in seconds.

var preferredIOBufferDuration: TimeInterval

The preferred I/O buffer duration, in seconds.

func setPreferredIOBufferDuration(TimeInterval) throws

Sets the preferred audio I/O buffer duration.

### Inspecting latency

var inputLatency: TimeInterval

The latency for audio input, in seconds.

var outputLatency: TimeInterval

The latency for audio output, in seconds.

### Inspecting output volume

var outputVolume: Float

The systemwide output volume set by the user.

### Setting the number of input channels

var preferredInputNumberOfChannels: Int

The preferred number of input channels for the current route.

func setPreferredInputNumberOfChannels(Int) throws

Sets the preferred number of input channels for the current route.

var inputNumberOfChannels: Int

The number of audio input channels for the current route.

var maximumInputNumberOfChannels: Int

The maximum number of input channels available for the current audio route.

### Setting the number of output channels

var preferredOutputNumberOfChannels: Int

The preferred number of output channels for the current route.

func setPreferredOutputNumberOfChannels(Int) throws

Sets the preferred number of output channels for the current route.

var outputNumberOfChannels: Int

The number of audio output channels.

var maximumOutputNumberOfChannels: Int

The maximum number of output channels available for the current audio route.

### Configuring multichannel support

var supportsMultichannelContent: Bool

A Boolean value that indicates whether your app supplies multichannel audio content.

func setSupportsMultichannelContent(Bool) throws

Sets whether your app supplies multichannel audio content.


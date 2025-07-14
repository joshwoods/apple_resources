

- AVFAudio
- AVAudioSession
-  inputDataSources 

Instance Property

# inputDataSources

An array of available data sources for the audio session’s current input port.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var inputDataSources: [AVAudioSessionDataSourceDescription]? { get }
```

## Discussion

This property returns an array of AVAudioSessionDataSourceDescription objects representing available input sources, or `nil` if switching between multiple input sources isn’t currently possible. Only certain devices and peripherals, such as an iPhone equipped with both front- and rear-facing microphones, support this feature.

You can observe changes to the value of this property by using key-value observing.

## See Also

### Configuring inputs

var isInputAvailable: Bool

A Boolean value that indicates whether an audio input path is available.

var availableInputs: [AVAudioSessionPortDescription]?

An array of input ports available for audio routing.

var preferredInput: AVAudioSessionPortDescription?

The preferred input port for audio routing.

func setPreferredInput(AVAudioSessionPortDescription?) throws

Sets the preferred input port for audio routing.

var inputDataSource: AVAudioSessionDataSourceDescription?

The currently selected input data source.

func setInputDataSource(AVAudioSessionDataSourceDescription?) throws

Selects a data source for the audio session’s current input port.


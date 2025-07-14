

- AVFAudio
- AVAudioSession
-  availableInputs 

Instance Property

# availableInputs

An array of input ports available for audio routing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var availableInputs: [AVAudioSessionPortDescription]? { get }
```

## Discussion

The active audio session category and mode determine the number of inputs this property returns. For example, if the session’s category is playAndRecord, the array may contain a built-in microphone port and, if connected, a headset microphone port. Alternatively, if the session’s category is playback, this property returns an empty array.

## See Also

### Configuring inputs

var isInputAvailable: Bool

A Boolean value that indicates whether an audio input path is available.

var preferredInput: AVAudioSessionPortDescription?

The preferred input port for audio routing.

func setPreferredInput(AVAudioSessionPortDescription?) throws

Sets the preferred input port for audio routing.

var inputDataSource: AVAudioSessionDataSourceDescription?

The currently selected input data source.

var inputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available data sources for the audio session’s current input port.

func setInputDataSource(AVAudioSessionDataSourceDescription?) throws

Selects a data source for the audio session’s current input port.


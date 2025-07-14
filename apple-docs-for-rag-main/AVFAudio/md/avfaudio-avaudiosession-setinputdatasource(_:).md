

- AVFAudio
- AVAudioSession
-  setInputDataSource(\_:) 

Instance Method

# setInputDataSource(\_:)

Selects a data source for the audio session’s current input port.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func setInputDataSource(_ dataSource: AVAudioSessionDataSourceDescription?) throws
```

## Parameters 

`dataSource`  

The data source for the audio session’s input.

## Discussion

You can set the input source to exactly one of the AVAudioSessionDataSourceDescription objects in the inputDataSources array. Only certain devices and peripherals, such as an iPhone equipped with both front- and rear-facing microphones, support switching among input sources.

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

var inputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available data sources for the audio session’s current input port.


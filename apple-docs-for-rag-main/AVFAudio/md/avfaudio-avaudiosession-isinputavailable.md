

- AVFAudio
- AVAudioSession
-  isInputAvailable 

Instance Property

# isInputAvailable

A Boolean value that indicates whether an audio input path is available.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isInputAvailable: Bool { get }
```

## Return Value

true if an input route is available, otherwise false.

## Discussion

Use this property to determine whether the device currently supports audio input.

This property is key-value observable.

## See Also

### Configuring inputs

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

func setInputDataSource(AVAudioSessionDataSourceDescription?) throws

Selects a data source for the audio session’s current input port.


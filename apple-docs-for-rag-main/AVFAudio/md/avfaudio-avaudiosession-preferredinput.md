

- AVFAudio
- AVAudioSession
-  preferredInput 

Instance Property

# preferredInput

The preferred input port for audio routing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var preferredInput: AVAudioSessionPortDescription? { get }
```

## Discussion

The value of this property indicates the input port selected using the setPreferredInput(_:) method. To see the actual current input port, use the currentRoute property. This property returns nil if you haven’t set a preference or if the previously set preferred input is no longer available.

## See Also

### Configuring inputs

var isInputAvailable: Bool

A Boolean value that indicates whether an audio input path is available.

var availableInputs: [AVAudioSessionPortDescription]?

An array of input ports available for audio routing.

func setPreferredInput(AVAudioSessionPortDescription?) throws

Sets the preferred input port for audio routing.

var inputDataSource: AVAudioSessionDataSourceDescription?

The currently selected input data source.

var inputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available data sources for the audio session’s current input port.

func setInputDataSource(AVAudioSessionDataSourceDescription?) throws

Selects a data source for the audio session’s current input port.




- AVFAudio
- AVAudioSession
-  setPreferredInput(\_:) 

Instance Method

# setPreferredInput(\_:)

Sets the preferred input port for audio routing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func setPreferredInput(_ inPort: AVAudioSessionPortDescription?) throws
```

## Parameters 

`inPort`  

An AVAudioSessionPortDescription object that describes the port to use for input.

## Discussion

Setting the preferred input port requests a change to the input audio route. To determine whether the change has taken effect, use the currentRoute property.

The value of the `inPort` parameter must be one of the AVAudioSessionPortDescription objects in the availableInputs array. If this parameter specifies a port that isn’t already part of the current audio route and the app’s session controls audio routing, this method initiates a route change to use the preferred port.

You must set a preferred input port only after setting the audio session’s category and mode and activating the session.

## See Also

### Configuring inputs

var isInputAvailable: Bool

A Boolean value that indicates whether an audio input path is available.

var availableInputs: [AVAudioSessionPortDescription]?

An array of input ports available for audio routing.

var preferredInput: AVAudioSessionPortDescription?

The preferred input port for audio routing.

var inputDataSource: AVAudioSessionDataSourceDescription?

The currently selected input data source.

var inputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available data sources for the audio session’s current input port.

func setInputDataSource(AVAudioSessionDataSourceDescription?) throws

Selects a data source for the audio session’s current input port.


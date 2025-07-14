

- AVFAudio
- AVAudioSession
-  setOutputDataSource(\_:) 

Instance Method

# setOutputDataSource(\_:)

Sets the output data source for an audio session.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func setOutputDataSource(_ dataSource: AVAudioSessionDataSourceDescription?) throws
```

## Parameters 

`dataSource`  

The data source for the audio session’s output.

## Discussion

You can change the output source to one of the AVAudioSessionDataSourceDescription objects in the outputDataSources array. Only certain USB accessories support this feature.

## See Also

### Configuring outputs

var outputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available output data sources for the current audio route.

var outputDataSource: AVAudioSessionDataSourceDescription?

The currently selected output data source.

class AVAudioSessionDataSourceDescription

An object that defines a data source for an audio input or output, giving information such as the source’s name, location, and orientation.

func overrideOutputAudioPort(AVAudioSession.PortOverride) throws

Temporarily changes the current audio route.


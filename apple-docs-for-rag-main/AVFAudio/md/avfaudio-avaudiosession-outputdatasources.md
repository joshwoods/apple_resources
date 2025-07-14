

- AVFAudio
- AVAudioSession
-  outputDataSources 

Instance Property

# outputDataSources

An array of available output data sources for the current audio route.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var outputDataSources: [AVAudioSessionDataSourceDescription]? { get }
```

## Discussion

This property returns an array of AVAudioSessionDataSourceDescription objects representing available output sources, or `nil` if switching between multiple output sources isn’t currently possible. Only certain USB accessories support this feature.

You can observe changes to the value of this property by using key-value observing.

## See Also

### Configuring outputs

var outputDataSource: AVAudioSessionDataSourceDescription?

The currently selected output data source.

func setOutputDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the output data source for an audio session.

class AVAudioSessionDataSourceDescription

An object that defines a data source for an audio input or output, giving information such as the source’s name, location, and orientation.

func overrideOutputAudioPort(AVAudioSession.PortOverride) throws

Temporarily changes the current audio route.


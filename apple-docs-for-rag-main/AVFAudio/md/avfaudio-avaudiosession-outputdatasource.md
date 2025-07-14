

- AVFAudio
- AVAudioSession
-  outputDataSource 

Instance Property

# outputDataSource

The currently selected output data source.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var outputDataSource: AVAudioSessionDataSourceDescription? { get }
```

## Discussion

The value of this property is nil if switching between multiple output sources isn’t currently possible. Only certain USB accessories support switching output sources.

## See Also

### Configuring outputs

var outputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available output data sources for the current audio route.

func setOutputDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the output data source for an audio session.

class AVAudioSessionDataSourceDescription

An object that defines a data source for an audio input or output, giving information such as the source’s name, location, and orientation.

func overrideOutputAudioPort(AVAudioSession.PortOverride) throws

Temporarily changes the current audio route.


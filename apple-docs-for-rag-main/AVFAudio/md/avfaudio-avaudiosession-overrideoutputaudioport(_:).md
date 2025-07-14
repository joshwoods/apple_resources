

- AVFAudio
- AVAudioSession
-  overrideOutputAudioPort(\_:) 

Instance Method

# overrideOutputAudioPort(\_:)

Temporarily changes the current audio route.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func overrideOutputAudioPort(_ portOverride: AVAudioSession.PortOverride) throws
```

## Parameters 

`portOverride`  

The override option for audio output. For a list of constants, see AVAudioSession.PortOverride.

## Discussion

If your app uses the playAndRecord category, calling this method with the AVAudioSession.PortOverride.speaker option causes the system to route audio to the built-in speaker and microphone regardless of other settings. This change remains in effect only until the current route changes or you call this method again with the AVAudioSession.PortOverride.none option.

If you’d prefer to permanently enable this behavior, you should instead set the category’s defaultToSpeaker option. Setting this option routes to the speaker rather than the receiver if no other accessory such as headphones are in use.

Note

The preferred method for routing audio to the speaker instead of the receiver for speakerphone functionality is through the use of the Media Player framework’s MPVolumeView class.

## Topics

### Data Types

enum PortOverride

Constants for use with the overrideOutputAudioPort(_:) method.

## See Also

### Configuring outputs

var outputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available output data sources for the current audio route.

var outputDataSource: AVAudioSessionDataSourceDescription?

The currently selected output data source.

func setOutputDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the output data source for an audio session.

class AVAudioSessionDataSourceDescription

An object that defines a data source for an audio input or output, giving information such as the source’s name, location, and orientation.


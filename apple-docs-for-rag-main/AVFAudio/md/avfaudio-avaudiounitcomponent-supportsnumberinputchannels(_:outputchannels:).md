

- AVFAudio
- AVAudioUnitComponent
-  supportsNumberInputChannels(\_:outputChannels:) 

Instance Method

# supportsNumberInputChannels(\_:outputChannels:)

Gets a Boolean value that indicates whether the audio unit component supports the specified number of input and output channels.

macOS 10.10+

``` source
func supportsNumberInputChannels(
    _ numInputChannels: Int,
    outputChannels numOutputChannels: Int
) -> Bool
```

## Parameters 

`numInputChannels`  

The number of input channels.

`numOutputChannels`  

The number of output channels.

## Return Value

A value of true if the audio unit component supports the specified number of input and output channels; otherwise, false.

## See Also

### Getting audio unit component information

var audioComponentDescription: AudioComponentDescription

The audio component description.

var availableArchitectures: [NSNumber]

An array of architectures that the audio unit supports.

var configurationDictionary: [String : Any]

The audio unit component’s configuration dictionary.

var hasCustomView: Bool

A Boolean value that indicates whether the audio unit component has a custom view.

var hasMIDIInput: Bool

A Boolean value that indicates whether the audio unit component has MIDI input.

var hasMIDIOutput: Bool

A Boolean value that indicates whether the audio unit component has MIDI output.

var manufacturerName: String

The name of the manufacturer of the audio unit component.

var name: String

The name of the audio unit component.

var passesAUVal: Bool

A Boolean value that indicates whether the audio unit component passes the validation tests.

var isSandboxSafe: Bool

A Boolean value that indicates whether the audio unit component is safe for sandboxing.

var typeName: String

The audio unit component type.

var version: Int

The audio unit component version number.

var versionString: String

A string that represents the audio unit component version number.

var componentURL: URL?

The URL of the audio unit component.

Deprecated


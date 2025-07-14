

- AVFAudio
- AVAudioUnitComponent
-  configurationDictionary 

Instance Property

# configurationDictionary

The audio unit component’s configuration dictionary.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+visionOS 1.0+

``` source
var configurationDictionary: [String : Any] { get }
```

## See Also

### Getting audio unit component information

var audioComponentDescription: AudioComponentDescription

The audio component description.

var availableArchitectures: [NSNumber]

An array of architectures that the audio unit supports.

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

func supportsNumberInputChannels(Int, outputChannels: Int) -> Bool

Gets a Boolean value that indicates whether the audio unit component supports the specified number of input and output channels.

var typeName: String

The audio unit component type.

var version: Int

The audio unit component version number.

var versionString: String

A string that represents the audio unit component version number.

var componentURL: URL?

The URL of the audio unit component.

Deprecated


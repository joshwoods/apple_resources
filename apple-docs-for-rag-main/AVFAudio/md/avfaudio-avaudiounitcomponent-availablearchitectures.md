

- AVFAudio
- AVAudioUnitComponent
-  availableArchitectures 

Instance Property

# availableArchitectures

An array of architectures that the audio unit supports.

macOS 10.10+

``` source
var availableArchitectures: [NSNumber] { get }
```

## Discussion

This is an `NSArray` of `NSNumbers` where each entry corresponds to one of the constants in Mach-O Architecture in Bundle.

## See Also

### Getting audio unit component information

var audioComponentDescription: AudioComponentDescription

The audio component description.

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




- Audio Toolbox
- AUAudioUnit
-  factoryPresets 

Instance Property

# factoryPresets

A collection of presets provided by the audio unit’s developer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var factoryPresets: [AUAudioUnitPreset]? { get }
```

## Discussion

A preset provides audio unit users with an easily-selectable, fine-tuned set of parameters defined by the developer.

This version 3 property is bridged to the version 2 `kAudioUnitProperty_FactoryPresets` API.

## See Also

### Managing Presets

var fullState: [String : Any]?

A persistable snapshot of the audio unit’s properties and parameters, suitable for saving as a user preset.

var fullStateForDocument: [String : Any]?

A persistable snapshot of the audio unit’s properties and parameters, suitable for saving in a user’s document.

var currentPreset: AUAudioUnitPreset?

The audio unit’s last-selected preset.

var supportsUserPresets: Bool

var userPresets: [AUAudioUnitPreset]

func saveUserPreset(AUAudioUnitPreset) throws

func deleteUserPreset(AUAudioUnitPreset) throws

func presetState(for: AUAudioUnitPreset) throws -> [String : Any]


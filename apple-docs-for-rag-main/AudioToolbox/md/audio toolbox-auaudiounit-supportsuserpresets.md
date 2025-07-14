

- Audio Toolbox
- AUAudioUnit
-  supportsUserPresets 

Instance Property

# supportsUserPresets

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var supportsUserPresets: Bool { get }
```

## See Also

### Managing Presets

var fullState: [String : Any]?

A persistable snapshot of the audio unit’s properties and parameters, suitable for saving as a user preset.

var fullStateForDocument: [String : Any]?

A persistable snapshot of the audio unit’s properties and parameters, suitable for saving in a user’s document.

var factoryPresets: [AUAudioUnitPreset]?

A collection of presets provided by the audio unit’s developer.

var currentPreset: AUAudioUnitPreset?

The audio unit’s last-selected preset.

var userPresets: [AUAudioUnitPreset]

func saveUserPreset(AUAudioUnitPreset) throws

func deleteUserPreset(AUAudioUnitPreset) throws

func presetState(for: AUAudioUnitPreset) throws -> [String : Any]


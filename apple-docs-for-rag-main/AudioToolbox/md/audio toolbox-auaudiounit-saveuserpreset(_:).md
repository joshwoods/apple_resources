

- Audio Toolbox
- AUAudioUnit
-  saveUserPreset(\_:) 

Instance Method

# saveUserPreset(\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func saveUserPreset(_ userPreset: AUAudioUnitPreset) throws
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

var supportsUserPresets: Bool

var userPresets: [AUAudioUnitPreset]

func deleteUserPreset(AUAudioUnitPreset) throws

func presetState(for: AUAudioUnitPreset) throws -> [String : Any]


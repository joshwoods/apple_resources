

- Audio Toolbox
- AUAudioUnit
-  currentPreset 

Instance Property

# currentPreset

The audio unit’s last-selected preset.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var currentPreset: AUAudioUnitPreset? { get set }
```

## Discussion

Hosts can let the user select a preset by setting this property. When getting this property, the preset does not reflect whether parameters may have been modified since it was selected.

This version 3 property is bridged to the version 2 `kAudioUnitProperty_PresentPreset` API.

## See Also

### Managing Presets

var fullState: [String : Any]?

A persistable snapshot of the audio unit’s properties and parameters, suitable for saving as a user preset.

var fullStateForDocument: [String : Any]?

A persistable snapshot of the audio unit’s properties and parameters, suitable for saving in a user’s document.

var factoryPresets: [AUAudioUnitPreset]?

A collection of presets provided by the audio unit’s developer.

var supportsUserPresets: Bool

var userPresets: [AUAudioUnitPreset]

func saveUserPreset(AUAudioUnitPreset) throws

func deleteUserPreset(AUAudioUnitPreset) throws

func presetState(for: AUAudioUnitPreset) throws -> [String : Any]


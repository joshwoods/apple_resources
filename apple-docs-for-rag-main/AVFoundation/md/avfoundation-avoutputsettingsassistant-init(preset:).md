

- AVFoundation
- AVOutputSettingsAssistant
-  init(preset:) 

Initializer

# init(preset:)

Creates an output setting assistant with a preset configuration.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
convenience init?(preset presetIdentifier: AVOutputSettingsPreset)
```

## Discussion

- presetIdentifier: A preset configuration for the object.

## See Also

### Creating an Assistant

struct AVOutputSettingsPreset

A structure that defines preset configurations for an output settings assistant.

class func availableOutputSettingsPresets() -> [AVOutputSettingsPreset]

Returns an array of preset values to use to initialize an output settings assistant.


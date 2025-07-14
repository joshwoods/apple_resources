

- AVFoundation
- AVOutputSettingsAssistant
-  availableOutputSettingsPresets() 

Type Method

# availableOutputSettingsPresets()

Returns an array of preset values to use to initialize an output settings assistant.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class func availableOutputSettingsPresets() -> [AVOutputSettingsPreset]
```

## Return Value

An array of available output settings presets.

## See Also

### Creating an Assistant

convenience init?(preset: AVOutputSettingsPreset)

Creates an output setting assistant with a preset configuration.

struct AVOutputSettingsPreset

A structure that defines preset configurations for an output settings assistant.


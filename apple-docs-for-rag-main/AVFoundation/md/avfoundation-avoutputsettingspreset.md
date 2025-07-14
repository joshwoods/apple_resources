

- AVFoundation
-  AVOutputSettingsPreset 

Structure

# AVOutputSettingsPreset

A structure that defines preset configurations for an output settings assistant.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVOutputSettingsPreset
```

## Topics

### Presets

static let preset3840x2160: AVOutputSettingsPreset

A preset for H.264 video at 3840 by 2160 pixels.

static let preset1920x1080: AVOutputSettingsPreset

A preset for H.264 video at 1920 by 1080 pixels.

static let preset1280x720: AVOutputSettingsPreset

A preset for H.264 video at 1280 by 720 pixels.

static let preset960x540: AVOutputSettingsPreset

A preset for H.264 video at 960 by 540 pixels.

static let preset640x480: AVOutputSettingsPreset

A preset for H.264 video at 640 by 480 pixels.

static let hevc7680x4320: AVOutputSettingsPreset

A preset for HEVC video at 7680 by 4320 pixels.

static let hevc3840x2160: AVOutputSettingsPreset

A preset for HEVC video at 3840 by 2160 pixels.

static let hevc3840x2160WithAlpha: AVOutputSettingsPreset

A preset for HEVC with Alpha video at 3840 by 2160 pixels.

static let hevc1920x1080: AVOutputSettingsPreset

A preset for HEVC video at 1920 by 1080 pixels.

static let hevc1920x1080WithAlpha: AVOutputSettingsPreset

A preset for HEVC with Alpha video at 1920 by 1080 pixels.

static let mvhevc1440x1440: AVOutputSettingsPreset

A preset for MV-HEVC video at 1440 by 1440 pixels.

static let mvhevc960x960: AVOutputSettingsPreset

A preset for MV-HEVC video at 960 by 960 pixels.

### Initializers

init(rawValue: String)

Creates a preset with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating an Assistant

convenience init?(preset: AVOutputSettingsPreset)

Creates an output setting assistant with a preset configuration.

class func availableOutputSettingsPresets() -> [AVOutputSettingsPreset]

Returns an array of preset values to use to initialize an output settings assistant.


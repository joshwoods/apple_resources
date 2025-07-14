

- AVFoundation
-  AVCaptionSettingsKey 

Structure

# AVCaptionSettingsKey

A structure that defines dictionary keys to configure the caption converter and validator.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct AVCaptionSettingsKey
```

## Topics

### Keys

static let mediaType: AVCaptionSettingsKey

A key that identifies the output media type of a caption conversion operation.

static let mediaSubType: AVCaptionSettingsKey

A key that identifies the output media subtype of a caption conversion operation.

static let timeCodeFrameDuration: AVCaptionSettingsKey

A key that identifies the frame duration that the system uses for the time code.

static let useDropFrameTimeCode: AVCaptionSettingsKey

A key that identifies whether the system uses drop frame time code.

### Initializers

init(rawValue: String)

Creates a settings key with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Conversion and Validation

class AVCaptionFormatConformer

An object that converts a canonical caption to a specific format.

class AVCaptionConversionValidator

An object that validates captions for a conversion operation.


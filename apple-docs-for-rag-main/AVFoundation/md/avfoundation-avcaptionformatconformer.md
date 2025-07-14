

- AVFoundation
-  AVCaptionFormatConformer 

Class

# AVCaptionFormatConformer

An object that converts a canonical caption to a specific format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionFormatConformer
```

## Topics

### Creating a Format Conformer

init(conversionSettings: [AVCaptionSettingsKey : Any])

Creates a new object with format conversion settings.

### Conforming Captions

var conformsCaptionsToTimeRange: Bool

A Boolean value that indicates whether to conform the time range of a canonical caption.

func conformedCaption(for: AVCaption) throws -> AVCaption

Creates a caption that conforms to a specific format.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Conversion and Validation

struct AVCaptionSettingsKey

A structure that defines dictionary keys to configure the caption converter and validator.

class AVCaptionConversionValidator

An object that validates captions for a conversion operation.


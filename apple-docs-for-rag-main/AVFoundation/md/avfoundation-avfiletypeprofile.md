

- AVFoundation
-  AVFileTypeProfile 

Structure

# AVFileTypeProfile

File type profiles for streaming formats.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVFileTypeProfile
```

## Topics

### File Type Profiles

static let mpeg4AppleHLS: AVFileTypeProfile

A file type profile for Apple HTTP Live Streaming.

static let mpeg4CMAFCompliant: AVFileTypeProfile

A file type profile that complies with the Common Media Application Format (CMAF).

### Initializers

init(rawValue: String)

Creates a file type profile from its raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### File types

struct AVFileType

The uniform type identifiers for various file formats.


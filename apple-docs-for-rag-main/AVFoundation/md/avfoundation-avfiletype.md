

- AVFoundation
-  AVFileType 

Structure

# AVFileType

The uniform type identifiers for various file formats.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVFileType
```

## Mentioned in 

Exporting video to alternative formats

## Topics

### File Types

static let ac3: AVFileType

The UTI for the AC3 audio file format.

static let aifc: AVFileType

The UTI for the AIFC audio file format.

static let aiff: AVFileType

The UTI for the AIFF audio file format.

static let AHAP: AVFileType

The UTI for the Apple Haptics Audio Pattern file format.

static let amr: AVFileType

The UTI for the adaptive multirate audio file format.

static let appleiTT: AVFileType

The UTI for the Apple iTT caption file format.

static let au: AVFileType

The UTI for the Sun/NeXT audio file format.

static let avci: AVFileType

The UTI for the high-efficiency image file format that contains H.264 compressed images.

static let caf: AVFileType

The UTI for the Core Audio Format.

static let dng: AVFileType

The UTI for the Adobe Digital Negative file format.

static let eac3: AVFileType

The UTI for the enhanced AC3 audio file format.

static let heic: AVFileType

The UTI for the high-efficiency image file format that contains HEVC compressed images.

static let heif: AVFileType

The UTI for the high-efficiency image file format that contains compressed images from any codec.

static let jpg: AVFileType

The UTI for the JPEG (JFIF) format.

static let m4a: AVFileType

The UTI for the Apple m4a audio file format.

static let m4v: AVFileType

The UTI for the iTunes video file format.

static let mobile3GPP: AVFileType

The UTI for the 3GPP file format.

static let mobile3GPP2: AVFileType

The UTI for the 3GPP2 file format.

static let mov: AVFileType

The UTI for the QuickTime movie file format.

static let mp3: AVFileType

The UTI for the MPEG Audio Layer III file format.

static let mp4: AVFileType

The UTI for the MPEG-4 file format.

static let SCC: AVFileType

The UTI for the Scenarist closed-caption file format.

static let tif: AVFileType

The UTI for the tagged image file format.

static let wav: AVFileType

The UTI for the WAVE audio file format.

### Initializers

init(String)

Creates a file type with a string.

init(rawValue: String)

Creates a file type from its raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### File types

struct AVFileTypeProfile

File type profiles for streaming formats.


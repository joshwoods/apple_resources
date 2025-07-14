

- ShazamKit
-  SHMediaItemProperty 

Structure

# SHMediaItemProperty

Constants for the media item property names.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SHMediaItemProperty
```

## Topics

### Creating a property key

init(String)

Creates a property key for the specified property.

init(rawValue: String)

Creates a property key for the specified property.

### General media item property keys

static let title: SHMediaItemProperty

The key to access the title property of a media item.

static let subtitle: SHMediaItemProperty

The key to access the subtitle property of a media item.

static let artist: SHMediaItemProperty

The key to access the artist property of a media item.

static let artworkURL: SHMediaItemProperty

The key to access the artwork URL property of a media item.

static let videoURL: SHMediaItemProperty

The key to access the video URL property of a media item.

static let genres: SHMediaItemProperty

The key to access the genres property of a media item.

static let explicitContent: SHMediaItemProperty

The key to access the explicit content property of a media item.

static let ISRC: SHMediaItemProperty

The key to access the International Standard Recording Code (ISRC) property of a media item.

static let frequencySkewRanges: SHMediaItemProperty

The key to access the frequency skew ranges property of a media item.

static let creationDate: SHMediaItemProperty

The date the media item was created.

static let timeRanges: SHMediaItemProperty

The key to access the time ranges property of a media item.

### Apple Music property keys

static let appleMusicURL: SHMediaItemProperty

The key to access the Apple Music URL property of a media item.

static let appleMusicID: SHMediaItemProperty

The key to access the Apple Music ID of a media item.

### Shazam music catalog property keys

static let webURL: SHMediaItemProperty

The key to access the web URL property of a media item.

static let shazamID: SHMediaItemProperty

The key to access the Shazam ID property of a media item.

### Matched media item property keys

static let matchOffset: SHMediaItemProperty

The key to access the match offset property of a matched media item.

static let frequencySkew: SHMediaItemProperty

The key to access the frequency skew property of a matched media item.

### Type Properties

static let confidence: SHMediaItemProperty

The value ranges from 0.0 to 1.0, where 1.0 indicates the highest level of confidence.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with media item properties

subscript(SHMediaItemProperty) -> Any

Accesses the property for the specified key for reading.

var timeRanges: [Range&lt;TimeInterval>]

An array of ranges that indicate the offsets within the reference signature that this media item describes.

var frequencySkewRanges: [Range&lt;Float>]

An array of ranges that indicate the frequency skews in the reference signature that this media item describes.


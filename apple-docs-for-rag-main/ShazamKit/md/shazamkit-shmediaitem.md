

- ShazamKit
-  SHMediaItem 

Class

# SHMediaItem

An object that represents the metadata for a reference signature.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class SHMediaItem
```

## Overview

This class uses subscripting for the data elements of a custom media item that an existing property doesn’t already represent.

Add a readable custom property by extending SHMediaItemProperty with a key for that property, and by extending this class with a property that uses the key. The following code shows the extensions for an episode number:

```
// Add an episode number to the list of properties.
extension SHMediaItemProperty {
    static let episode = SHMediaItemProperty("Episode")
}

// Add a property for returning the episode number using a subscript.
extension SHMediaItem {
    var episode: Int? {
        return self[.episode] as? Int
    }
}
```

Add your custom property when you create the media item as the following code shows:

```
// Create a new media item and set the title, subtitle, and episode properties.
let mediaItem = SHMediaItem(properties: [.episode: 42,
                                         .title: "Question",
                                         .subtitle: "The Answer"])
```

Note

The class of the object that represents a custom object must be one of: `Dictionary`, `Array`, `URL`, `Number`, `String`, `Date`, or `Data`.

## Topics

### Creating a new media item object

convenience init(properties: [SHMediaItemProperty : Any])

Creates a media item object with a dictionary of properties and their associated values.

### Working with media item properties

subscript(SHMediaItemProperty) -> Any

Accesses the property for the specified key for reading.

struct SHMediaItemProperty

Constants for the media item property names.

var timeRanges: [Range&lt;TimeInterval>]

An array of ranges that indicate the offsets within the reference signature that this media item describes.

var frequencySkewRanges: [Range&lt;Float>]

An array of ranges that indicate the frequency skews in the reference signature that this media item describes.

### Reading general media item properties

var title: String?

A title for the media item.

var subtitle: String?

A subtitle for the media item.

var artist: String?

The name of the artist for the media item, such as the performer of a song.

var artworkURL: URL?

The URL for artwork for the media item, such as an album cover.

var videoURL: URL?

The URL for a video for the media item, such as a music video.

var genres: [String]

An array of genre names for the media item.

var explicitContent: Bool

A Boolean value that indicates whether the media item contains explicit content.

var creationDate: Date?

The date the media item was created.

var isrc: String?

The International Standard Recording Code (ISRC) for the media item.

var id: UUID

A unique identifier for this media item.

### Reading Apple Music properties

var songs: [Song]

An array of MusicKit song objects that represent the song.

var appleMusicURL: URL?

A link to the Apple Music page that contains the full information for the song.

var appleMusicID: String?

The Apple Music ID for the song.

### Working with Shazam music catalog media items

var webURL: URL?

A link to the Shazam Music catalog page that contains the full information for the song.

var shazamID: String?

The Shazam ID for the song.

class func fetch(shazamID: String, completionHandler: (SHMediaItem?, (any Error)?) -> Void)

Requests the media item for the song with the specified Shazam ID.

### Default Implementations

Identifiable Implementations

## Relationships

### Inherits From

- NSObject

### Inherited By

- SHMatchedMediaItem

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Match audio

class SHSession

An object that matches a specific audio recording when a segment of that recording is part of captured sound in the Shazam catalog or your custom catalog.

class SHManagedSession

An object that records and matches a recording with captured sound in the Shazam catalog or your custom catalog.

protocol SHSessionDelegate

Methods that the session calls with the result of a match request.

class SHMatch

An object that represents the catalog media items that match a query.

class SHMatchedMediaItem

An object that represents the metadata for a matched reference signature.


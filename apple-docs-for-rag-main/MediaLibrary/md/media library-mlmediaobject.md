

- Media Library
-  MLMediaObject 

Class

# MLMediaObject

The `MLMediaObject` class describes a single media file, such as a photo, song, or movie. Each media object contains basic metadata including a name, media type, URL, and so on. Additional information about each object is stored in its list of attributes. For a list of possible object attribute keys, see Media Object Attribute Keys.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
class MLMediaObject
```

## Overview

A media object belongs to a single media source but can be referenced by several groups within that source. In other words, an object can appear in multiple places in the group hierarchy under a single media source. In iTunes, a movie that was purchased through the iTunes Store is referenced by both the Purchased playlist and the Movies playlist. If a user adds the movie to his own playlist, the group respresenting that playlist will also reference the movie. All three groups reference the same media object.

All `MLMediaObject` properties are read-only, so this information can be accessed but not altered.

## Topics

### Identifying the Object

var identifier: String

An identifier for the media object.

var mediaSourceIdentifier: String

An identifier for the source that loaded the media object.

var mediaLibrary: MLMediaLibrary?

A pointer to the media library instance that loaded the media object’s source.

### Accessing Object Attributes

var attributes: [String : Any]

A dictionary of attributes describing the media object.

var mediaType: MLMediaType

The media object’s type of media (image, audio, or movie).

var contentType: String?

The UTI associated with the media object.

var name: String?

The name of the media object.

var url: URL?

The location of the media object.

var originalURL: URL?

The location of the original media object, if url is not the original location.

var fileSize: Int

The size, in bytes, of the media object.

var modificationDate: Date?

The date and time when the media object was last altered.

var thumbnailURL: URL?

The location of the media object’s thumbnail image.

var artworkImage: NSImage?

Album artwork associated with the media object.

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

### Classes

class MLMediaGroup

The `MLMediaGroup` class provides groupings for media objects from a single source of media, such as iTunes or Aperture. The media objects—individual files containing a piece of media such as a photo, song, or movie—are referenced by one or more groups within each media source. These groupings serve as filters, providing hierarchical structure to the collection of objects in each source.

class MLMediaLibrary

The `MLMediaLibrary` class provides an interface for accessing a collection of media objects from various sources. It serves as the initial access point of the Media Library framework.

class MLMediaSource

The `MLMediaSource` class identifies a specific provider of media. Conceptually, a media source respresents a single app, such as iTunes or Aperture. Each media source contains multiple groups of media objects—individual files containing a piece of media such as a photo, song, or movie.


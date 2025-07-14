

- Media Library
- MLMediaObject
-  artworkImage 

Instance Property

# artworkImage

Album artwork associated with the media object.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
@NSCopying
var artworkImage: NSImage? { get }
```

## Discussion

Applies to iTunes media only. Returns `nil` if not applicable or not available.

## See Also

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


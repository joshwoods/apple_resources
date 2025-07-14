

- Media Library
- MLMediaObject
-  originalURL 

Instance Property

# originalURL

The location of the original media object, if url is not the original location.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
var originalURL: URL? { get }
```

## Discussion

This property is provided as a security-scoped URL. In order to gain access to the file that this URL refers to, the caller must call startAccessingSecurityScopedResource() before and stopAccessingSecurityScopedResource() after using the URL to access the file. For more information about security-scoped URLs, see NSURL.

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

var fileSize: Int

The size, in bytes, of the media object.

var modificationDate: Date?

The date and time when the media object was last altered.

var thumbnailURL: URL?

The location of the media object’s thumbnail image.

var artworkImage: NSImage?

Album artwork associated with the media object.


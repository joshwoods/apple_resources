

- Media Player
-  MPMediaItemArtwork 

Class

# MPMediaItemArtwork

A graphical image, such as music album cover art, associated with a media item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
class MPMediaItemArtwork
```

## Topics

### Resizing existing artwork

init(boundsSize: CGSize, requestHandler: (CGSize) -> UIImage)

Creates a new image from existing artwork with the specified bounds.

### Using a media item image

func image(at: CGSize) -> UIImage?

Returns the artwork image for an item at the given size.

var bounds: CGRect

The maximum size, in points, of the image associated with the media item artwork.

### Initializers

convenience init(image: UIImage)

Initializes a media item artwork instance with a full-size image.

Deprecated

### Instance Properties

var imageCropRect: CGRect

The bounds, in points, of the content area for the full size image associated with the media item artwork.

Deprecated

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

### Media items and playlists

class MPMediaItem

A collection of properties that represents a single item in the media library.

class MPMediaItemCollection

A sorted set of media items from the media library.

class MPMediaPlaylist

A playable collection of related media items.

class MPMediaPlaylistCreationMetadata

A set of attributes for describing a playlist when creating it.

class MPMediaEntity

The abstract superclass for media items, media item collections, and media playlist instances.


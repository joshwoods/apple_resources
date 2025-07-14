

- MusicKit
-  Artwork 

Structure

# Artwork

An object that represents artwork for a music item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Artwork
```

## Topics

### Operators

static func == (Artwork, Artwork) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let alternateText: String?

A textual description for the image.

let backgroundColor: CGColor?

The average background color of the image.

var hashValue: Int

The hash value.

let maximumHeight: Int

The maximum height available for the image.

let maximumWidth: Int

The maximum width available for the image.

let primaryTextColor: CGColor?

The primary text color to use when displaying the background color.

let quaternaryTextColor: CGColor?

The final posttertiary text color to use when displaying the background color.

let secondaryTextColor: CGColor?

The secondary text color to use when displaying the background color.

let tertiaryTextColor: CGColor?

The tertiary text color to use when displaying the background color.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

func url(width: Int, height: Int) -> URL?

Returns a URL to request the image asset for a specified width and height.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Artwork

struct ArtworkImage

A view that displays the image for a music item’s artwork.


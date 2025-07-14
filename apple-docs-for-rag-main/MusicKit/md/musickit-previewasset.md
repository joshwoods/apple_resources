

- MusicKit
-  PreviewAsset 

Structure

# PreviewAsset

An object that represents a preview for resources.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct PreviewAsset
```

## Topics

### Operators

static func == (PreviewAsset, PreviewAsset) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let artwork: Artwork?

The preview artwork for the associated preview music video.

var hashValue: Int

The hash value.

let hlsURL: URL?

The HLS preview URL for the content.

let url: URL?

The preview URL for the content.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

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

### Music Item Attributes

enum ContentRating

The rating of the content that potentially plays while playing a resource.

struct EditorialNotes

An object that represents editorial notes.


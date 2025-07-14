

- MusicKit
-  EditorialNotes 

Structure

# EditorialNotes

An object that represents editorial notes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct EditorialNotes
```

## Topics

### Operators

static func == (EditorialNotes, EditorialNotes) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let name: String?

The name for the editorial notes.

let short: String?

Abbreviated notes that display inline or when the content appears alongside other content.

let standard: String?

Notes that appear when the content displays prominently.

let tagline: String?

The tag line for the editorial notes.

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

struct PreviewAsset

An object that represents a preview for resources.


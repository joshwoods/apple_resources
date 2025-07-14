

- TV Services
-  TVContentIdentifier Deprecated

Class

# TVContentIdentifier

An object that uniquely identifies media content in either a single piece or a collection.

tvOS 9.0–13.0Deprecated

``` source
class TVContentIdentifier
```

Deprecated

TVContentIdentifier has been replaced by TVTopShelfContentProvider

## Overview

Every content identifier is represented by two parts: a string identifier (identifier) and a container identifier (container). The container identifier may be `nil`, which indicates that the content lives at the top level of the container hierarchy. You are responsible for organizing your content into a hierarchy and creating identifiers that uniquely identify each piece of content.

When designing your content identifiers, follow this guidance:

- A given content identifier must be unique for a particular content item, across *all* past, current, and future content items, even if the user no longer has access to that item.

- The uniqueness of a content identifier comes from the uniqueness of its two parts. The identifier property of a content identifier need not be universally unique across all of the app’s content identifiers, as long as items that share the same identifier string are contained in different containers.

## Topics

### Initializing a Content Identifier

init(identifier: String, container: TVContentIdentifier?)

Creates a new content identifier.

init?(coder: NSCoder)

Returns an object initialized from data in a given unarchiver.

### Inspecting an Identifier’s Contents

var identifier: String

The string that identifies this content item.

var container: TVContentIdentifier?

The container that this content item is contained in.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Content

class TVContentItem

An object that describes either a piece of content or a container for other content items.

Deprecated

func TVTopShelfImageSize(shape: TVContentItemImageShape, style: TVTopShelfContentStyle) -> CGSize

Returns the ideal size for an image, according to its particular shape and style.

Deprecated


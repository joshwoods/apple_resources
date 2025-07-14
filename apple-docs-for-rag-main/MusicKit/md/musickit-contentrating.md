

- MusicKit
-  ContentRating 

Enumeration

# ContentRating

The rating of the content that potentially plays while playing a resource.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum ContentRating
```

## Overview

A nil value means no rating is available for this resource.

## Topics

### Operators

static func == (ContentRating, ContentRating) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case clean

case explicit

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Music Item Attributes

struct EditorialNotes

An object that represents editorial notes.

struct PreviewAsset

An object that represents a preview for resources.


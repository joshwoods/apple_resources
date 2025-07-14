

- AVFoundation
-  AVMetadataItemFilter 

Class

# AVMetadataItemFilter

An object that filters selected information from a metadata item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMetadataItemFilter
```

## Overview

Filter instances are opaque, unmodifiable objects, that you create with the forSharing() class method.

## Topics

### Creating a Metadata Item Filter

class func forSharing() -> AVMetadataItemFilter

Returns a metadata filter to use for sharing assets.

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
- Sendable

## See Also

### Metadata

Retrieving media metadata

Load descriptive metadata for media assets and their tracks.

class AVMetadataItem

A metadata item for an audiovisual asset or one of its tracks.

class AVMutableMetadataItem

A mutable metadata item for an audiovisual asset or for one of its tracks.

struct AVMetadataIdentifier

A structure that defines identifiers for metadata formats.

struct AVMetadataKey

A structure that defines a metadata key.

struct AVMetadataKeySpace

A structure that defines a metadata key space.

struct AVMetadataExtraAttributeKey

A structure that defines keys for extra metadata attributes.

struct AVMetadataFormat

A structure that defines metadata formats.


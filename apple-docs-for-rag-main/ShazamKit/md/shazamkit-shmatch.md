

- ShazamKit
-  SHMatch 

Class

# SHMatch

An object that represents the catalog media items that match a query.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class SHMatch
```

## Overview

A single query signature may match more than one reference signature. In addition, one reference signature may map to many media items.

## Topics

### Reading match information

var mediaItems: [SHMatchedMediaItem]

An array of the media items in the catalog that match the query signature, in order of the quality of the match.

var querySignature: SHSignature

The query signature for the match.

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
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Match audio

class SHSession

An object that matches a specific audio recording when a segment of that recording is part of captured sound in the Shazam catalog or your custom catalog.

class SHManagedSession

An object that records and matches a recording with captured sound in the Shazam catalog or your custom catalog.

protocol SHSessionDelegate

Methods that the session calls with the result of a match request.

class SHMatchedMediaItem

An object that represents the metadata for a matched reference signature.

class SHMediaItem

An object that represents the metadata for a reference signature.


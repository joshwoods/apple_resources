

- ShazamKit
-  SHMatchedMediaItem 

Class

# SHMatchedMediaItem

An object that represents the metadata for a matched reference signature.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class SHMatchedMediaItem
```

## Overview

To access properties for custom media items, use subscripting. For more information, see SHMediaItem.

## Topics

### Reading information about the match

var matchOffset: TimeInterval

The timecode in the reference recording that matches the start of the query, in seconds.

var predictedCurrentMatchOffset: TimeInterval

The updated timecode in the reference recording that matches the current playback position of the query audio, in seconds.

var frequencySkew: Float

A multiple for the difference in frequency between the matched audio and the query audio.

### Instance Properties

var confidence: Float

The level of confidence in the match result.

## Relationships

### Inherits From

- SHMediaItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSCoding
- NSCopying
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

class SHMatch

An object that represents the catalog media items that match a query.

class SHMediaItem

An object that represents the metadata for a reference signature.


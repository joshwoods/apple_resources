

- MusicKit
-  MusicDataResponse 

Structure

# MusicDataResponse

An object containing results for a data request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicDataResponse
```

## Topics

### Operators

static func == (MusicDataResponse, MusicDataResponse) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let data: Data

The raw data returned by the Apple Music API endpoint for the originating data request.

var hashValue: Int

The hash value.

let urlResponse: HTTPURLResponse

The URL response returned by the Apple Music API endpoint for the originating data request.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### General Purpose Data Request

struct MusicDataRequest

A request for loading data from an arbitrary Apple Music API endpoint.


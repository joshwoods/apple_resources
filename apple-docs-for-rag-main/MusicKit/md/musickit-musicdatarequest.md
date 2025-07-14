

- MusicKit
-  MusicDataRequest 

Structure

# MusicDataRequest

A request for loading data from an arbitrary Apple Music API endpoint.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicDataRequest
```

## Topics

### Structures

struct Error

An error that the Apple Music API returns.

### Operators

static func == (MusicDataRequest, MusicDataRequest) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(urlRequest: URLRequest)

Creates a data request with a URL request.

### Instance Properties

var hashValue: Int

The hash value.

let urlRequest: URLRequest

The URL request for the data request.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

func response() async throws -> MusicDataResponse

Fetches data from the Apple Music API endpoint that the URL request defines.

### Type Properties

static var currentCountryCode: String

Fetches the current country code for the user’s Apple Music account.

static var tokenProvider: any MusicUserTokenProvider &amp; MusicDeveloperTokenProvider

The shared token provider for fetching tokens that Apple Music API requires.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### General Purpose Data Request

struct MusicDataResponse

An object containing results for a data request.


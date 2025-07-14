

- WeatherKit
-  WeatherError 

Enumeration

# WeatherError

An error WeatherKit returns.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum WeatherError
```

## Topics

### Getting the error type

case permissionDenied

An error indicating permission denied.

case unknown

An unknown error.

### Getting the error properties

var errorDescription: String?

A localized message describing what error occurred.

var failureReason: String?

A localized message describing the reason for the failure.

var helpAnchor: String?

A localized message providing text if the user requests help.

var recoverySuggestion: String?

A localized message describing how to recover from the failure.

### Operators

static func == (WeatherError, WeatherError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable


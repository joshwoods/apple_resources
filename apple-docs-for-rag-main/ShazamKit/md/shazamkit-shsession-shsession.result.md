

- ShazamKit
- SHSession
-  SHSession.Result 

Enumeration

# SHSession.Result

Identifies the result from an asynchronous sequence result.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
enum Result
```

## Topics

### Constants

case match(SHMatch)

A type that indicates a session match.

case noMatch(SHSignature)

A type that indicates there’s no match for the signature.

case error(any Error, SHSignature)

A type that indicates a session error.

## Relationships

### Conforms To

- Sendable

## See Also

### Returning queries

func result(from: SHSignature) async -> SHSession.Result

Performs an asynchronous match with a signature you specify.


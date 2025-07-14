

- ShazamKit
- SHSession
-  SHSession.Results 

Structure

# SHSession.Results

An asynchronous sequence that emits updates from a session object query.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Results
```

## Topics

### Creating an iterator

struct Iterator

An interator for accessing session results.

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Reading the session properties

var delegate: (any SHSessionDelegate)?

The object that the session calls with the result of a match request.

var catalog: SHCatalog

The catalog object containing the reference signatures and their associated metadata that the session uses to perform matches.

var results: SHSession.Results

The results as an asynchronous sequence of matches.




- Core Spotlight
- CSIndexError
-  CSIndexError.Code 

Enumeration

# CSIndexError.Code

Error codes that describe indexing-specific errors.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
enum Code
```

## Topics

### Getting the indexing error codes

case indexUnavailableError

The indexer is unavailable.

case indexingUnsupported

Indexing isn’t supported on the device.

case invalidClientStateError

The provided client state data is invalid.

case invalidItemError

The searchable item object is invalid.

case mismatchedClientState

The provided client state did not match the information in the index.

case quotaExceeded

The quota for the bundle has been exceeded.

case remoteConnectionError

An error occurred while communicating with the remote process.

case unknownError

An unknown error occurred.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable


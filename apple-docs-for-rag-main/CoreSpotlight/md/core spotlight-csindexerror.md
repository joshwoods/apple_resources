

- Core Spotlight
-  CSIndexError 

Structure

# CSIndexError

Index errors returned by Core Spotlight.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
struct CSIndexError
```

## Topics

### Getting the error codes

static var indexUnavailableError: CSIndexError.Code

The indexer is unavailable.

static var indexingUnsupported: CSIndexError.Code

Indexing isn’t supported on the device.

static var invalidClientStateError: CSIndexError.Code

The provided client state data is invalid.

static var invalidItemError: CSIndexError.Code

The searchable item object is invalid.

static var mismatchedClientState: CSIndexError.Code

The provided client state did not match the information in the index.

static var quotaExceeded: CSIndexError.Code

The quota for the bundle has been exceeded.

static var remoteConnectionError: CSIndexError.Code

An error occurred while communicating with the remote process.

static var unknownError: CSIndexError.Code

An unknown error occurred.

### Getting codes for indexing errors

enum Code

Error codes that describe indexing-specific errors.

### Getting the error description

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

struct CSSearchQueryError

Search query errors returned by Core Spotlight.

CSIndex Errors

Index error codes and error domain.

CSSearchQuery Errors

Search query error codes and error domain.


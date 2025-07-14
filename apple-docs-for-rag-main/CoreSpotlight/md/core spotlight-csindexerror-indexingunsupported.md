

- Core Spotlight
- CSIndexError
-  indexingUnsupported 

Type Property

# indexingUnsupported

Indexing isn’t supported on the device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
static var indexingUnsupported: CSIndexError.Code { get }
```

## See Also

### Getting the error codes

static var indexUnavailableError: CSIndexError.Code

The indexer is unavailable.

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


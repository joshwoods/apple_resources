

- Link Presentation
-  LPError 

Structure

# LPError

An error returned by the LinkPresentation framework.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
struct LPError
```

## Topics

### Error details

var errorCode: Int

A code for the error.

var errorUserInfo: [String : Any]

### Error domain

static var errorDomain: String

The domain for the error.

let LPErrorDomain: String

The domain for Link Presentation errors.

### Error codes

static var metadataFetchCancelled: LPError.Code

An error indicating that the metadata fetch was canceled by the client.

static var metadataFetchFailed: LPError.Code

An error indicating that a metadata fetch failed.

static var metadataFetchTimedOut: LPError.Code

An error indicating that the metadata fetch took longer than allowed.

static var unknown: LPError.Code

enum Code

Possible error values that can be returned from LinkPresentation APIs.

### Type Properties

static var metadataFetchNotAllowed: LPError.Code

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Possible error values that can be returned from LinkPresentation APIs.

let LPErrorDomain: String

The domain for Link Presentation errors.




- Link Presentation
- LPError
-  LPError.Code 

Enumeration

# LPError.Code

Possible error values that can be returned from LinkPresentation APIs.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error cases

case metadataFetchCancelled

An error indicating that the metadata fetch was canceled by the client.

case metadataFetchFailed

An error indicating that a metadata fetch failed.

case metadataFetchTimedOut

An error indicating that the metadata fetch took longer than allowed.

case unknown

An unknown error.

### Enumeration Cases

case metadataFetchNotAllowed

An error indicating that the metadata fetch was not allowed due to system policies.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct LPError

An error returned by the LinkPresentation framework.

let LPErrorDomain: String

The domain for Link Presentation errors.


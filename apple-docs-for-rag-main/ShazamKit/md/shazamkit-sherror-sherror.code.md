

- ShazamKit
- SHError
-  SHError.Code 

Enumeration

# SHError.Code

Codes for the errors that Shazam produces.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Code
```

## Topics

### Matching errors

case matchAttemptFailed

The error code to indicate when a Shazam Music catalog server issue prevents finding a match.

### Signature errors

case signatureInvalid

The error code to indicate that the system is unable to generate a signature from the audio.

case signatureDurationInvalid

The error code to indicate that the length of the generated signature is too long or too short to make a match in the catalog.

### Audio format errors

case invalidAudioFormat

The error code to indicate an unsupported audio format.

case audioDiscontinuity

The error code to indicate the use of noncontiguous audio to request a match.

### Catalog errors

case customCatalogInvalidURL

The error code to indicate that the format for the custom catalog URL is invalid.

case customCatalogInvalid

The error code to indicate when the custom catalog fails to load due to an invalid format.

### Library sync errors

case mediaItemFetchFailed

The error code to indicate when the system fails to fetch one or more media items.

case mediaLibrarySyncFailed

The error code to indicate when the system fails to add one or more media items to the user’s Shazam library.

### Framework errors

case internalError

The error code to indicate a generic framework error.

### Querying the error domain

let SHErrorDomain: String

The error domain for specific errors for ShazamKit.

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

### Inspecting an error

Error Constants

Error code constants for framework operations.


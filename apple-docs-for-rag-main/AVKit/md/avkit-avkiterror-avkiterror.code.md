

- AVKit
- AVKitError
-  AVKitError.Code 

Enumeration

# AVKitError.Code

Constants that identify framework error codes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error Codes

case unknown

An unknown error.

case contentRatingUnknown

The media content rating is missing or unrecognized.

case contentDisallowedByPasscode

A restriction disallows access to this content, but the user can override the restriction by entering the device passcode.

case pictureInPictureStartFailed

The system failed to start Picture in Picture.

case contentDisallowedByProfile

An installed profile restricts access to this content.

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

let AVKitErrorDomain: String

The domain of errors the framework generates.

struct AVKitError

A structure that represents a framework error.


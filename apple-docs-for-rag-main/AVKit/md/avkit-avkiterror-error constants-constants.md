

- AVKit
- AVKitError
-  Error Constants 

API Collection

# Error Constants

Error code constants for framework operations.

## Topics

### Error Code Constants

Error code constants for framework operations.

static var unknown: AVKitError.Code

An unknown error.

static var contentRatingUnknown: AVKitError.Code

The media content rating is missing or unrecognized.

static var contentDisallowedByPasscode: AVKitError.Code

A restriction disallows access to this content, but the user can override the restriction by entering the device passcode.

static var contentDisallowedByProfile: AVKitError.Code

An installed profile restricts access to this content.

static var pictureInPictureStartFailed: AVKitError.Code

The system failed to start Picture in Picture.

## See Also

### Inspecting an Error

static var errorDomain: String

enum Code

Constants that identify framework error codes.


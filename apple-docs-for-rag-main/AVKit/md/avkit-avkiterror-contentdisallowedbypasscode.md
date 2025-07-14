

- AVKit
- AVKitError
-  contentDisallowedByPasscode 

Type Property

# contentDisallowedByPasscode

A restriction disallows access to this content, but the user can override the restriction by entering the device passcode.

tvOS 13.0+

``` source
static var contentDisallowedByPasscode: AVKitError.Code { get }
```

## See Also

### Error Code Constants

static var unknown: AVKitError.Code

An unknown error.

static var contentRatingUnknown: AVKitError.Code

The media content rating is missing or unrecognized.

static var contentDisallowedByProfile: AVKitError.Code

An installed profile restricts access to this content.

static var pictureInPictureStartFailed: AVKitError.Code

The system failed to start Picture in Picture.


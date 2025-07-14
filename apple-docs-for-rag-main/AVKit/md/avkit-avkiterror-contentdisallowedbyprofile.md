

- AVKit
- AVKitError
-  contentDisallowedByProfile 

Type Property

# contentDisallowedByProfile

An installed profile restricts access to this content.

tvOS 13.0+

``` source
static var contentDisallowedByProfile: AVKitError.Code { get }
```

## Discussion

The user can’t override this restriction by entering the passcode, but they may be able to override it in the Settings app.

## See Also

### Error Code Constants

static var unknown: AVKitError.Code

An unknown error.

static var contentRatingUnknown: AVKitError.Code

The media content rating is missing or unrecognized.

static var contentDisallowedByPasscode: AVKitError.Code

A restriction disallows access to this content, but the user can override the restriction by entering the device passcode.

static var pictureInPictureStartFailed: AVKitError.Code

The system failed to start Picture in Picture.


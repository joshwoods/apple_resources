

- AVKit
- AVKitError
- AVKitError.Code
-  AVKitError.Code.contentDisallowedByProfile 

Case

# AVKitError.Code.contentDisallowedByProfile

An installed profile restricts access to this content.

tvOS 13.0+

``` source
case contentDisallowedByProfile
```

## Discussion

The user can’t override this restriction by entering the device passcode, but they may be able to override it in the Settings app.

## See Also

### Error Codes

case unknown

An unknown error.

case contentRatingUnknown

The media content rating is missing or unrecognized.

case contentDisallowedByPasscode

A restriction disallows access to this content, but the user can override the restriction by entering the device passcode.

case pictureInPictureStartFailed

The system failed to start Picture in Picture.


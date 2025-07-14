

- AVFoundation
- AVCaptureDevice
-  authorizationStatus(for:) 

Type Method

# authorizationStatus(for:)

Returns an authorization status that indicates whether the user grants the app permission to capture media of a particular type.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.14+tvOS 17.0+visionOS 1.0+

``` source
class func authorizationStatus(for mediaType: AVMediaType) -> AVAuthorizationStatus
```

## Parameters 

`mediaType`  

A media type for which to check the authorization status. The supported media types are video and audio.

## Return Value

An authorization status value.

## Mentioned in 

Requesting authorization to capture and save media

## Discussion

A user must explicitly grant your app access to record audio or video. Call this method to determine your app’s current authorization status. If it returns a value of AVAuthorizationStatus.notDetermined, call requestAccess(for:completionHandler:) to prompt the user for capture permission.

After the user grants permission, the system remembers their choice and doesn’t prompt them again. However, a user can change their choice at any time in the Settings app.

Note

If a user has denied your app recording permission, or hasn’t yet responded to the permission prompt, audio recordings contain only silence and video recordings contain only black frames.

## See Also

### Authorizing Device Access

class func requestAccess(for: AVMediaType, completionHandler: (Bool) -> Void)

Requests the user’s permission to allow the app to capture media of a particular type.

enum AVAuthorizationStatus

Constants that indicate the status of an app’s authorization to capture media.


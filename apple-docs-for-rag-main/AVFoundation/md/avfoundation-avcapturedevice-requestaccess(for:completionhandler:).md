

- AVFoundation
- AVCaptureDevice
-  requestAccess(for:completionHandler:) 

Type Method

# requestAccess(for:completionHandler:)

Requests the user’s permission to allow the app to capture media of a particular type.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.14+tvOS 17.0+visionOS 1.0+

``` source
class func requestAccess(
    for mediaType: AVMediaType,
    completionHandler handler: @escaping (Bool) -> Void
)
```

``` source
class func requestAccess(for mediaType: AVMediaType) async -> Bool
```

## Parameters 

`mediaType`  

A media type for which to check the authorization status. The supported media types are video and audio.

`handler`  

A callback the system invokes with a Boolean value that indicates whether the user granted or denied access to your app.

Return control to the main queue or MainActor before performing user interface updates.

## Mentioned in 

Requesting authorization to capture and save media

## Discussion

Capturing media requires explicit permission from the user. An app’s default authorization status is AVAuthorizationStatus.notDetermined, which means the user hasn’t yet granted it permission to capture media. The first time you create an AVCaptureDeviceInput object for a media type that requires permission, the system automatically displays an alert to request recording permission. Alternatively, call this method to prompt the user at a time of your choosing. The system saves the user’s selection so that it doesn’t have to prompt the user again. A user can change their authorization status in the Settings app.

Important

Your app must provide an explanation for its use of capture devices using the NSCameraUsageDescription and NSMicrophoneUsageDescription Info.plist keys. The system presents the strings you set for these keys when prompting the user for permission, and thereafter in the Settings app. Calling this method or attempting to start a capture session without a usage description raises an exception.

Calling this method doesn’t block the thread while the system is prompting the user for access. However, until the grants permission, the system only vends black video frames and silent audio samples.

Note

Calling this method with a media type of audio is equivalent to calling the requestRecordPermission(_:) method on AVAudioSession.

## See Also

### Authorizing Device Access

class func authorizationStatus(for: AVMediaType) -> AVAuthorizationStatus

Returns an authorization status that indicates whether the user grants the app permission to capture media of a particular type.

enum AVAuthorizationStatus

Constants that indicate the status of an app’s authorization to capture media.


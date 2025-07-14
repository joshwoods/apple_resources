

- Speech
- SFSpeechRecognizer
-  authorizationStatus() 

Type Method

# authorizationStatus()

Returns your app’s current authorization to perform speech recognition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class func authorizationStatus() -> SFSpeechRecognizerAuthorizationStatus
```

## Return Value

The app’s current authorization status value. For a list of values, see SFSpeechRecognizerAuthorizationStatus.

## Discussion

The user can reject your app’s request to perform speech recognition, but your request can also be denied if speech recognition is not supported on the device. The app can also change your app’s authorization status at any time from the Settings app.

## See Also

### Requesting Authorization from the User

class func requestAuthorization((SFSpeechRecognizerAuthorizationStatus) -> Void)

Asks the user to allow your app to perform speech recognition.

enum SFSpeechRecognizerAuthorizationStatus

The app’s authorization to perform speech recognition.


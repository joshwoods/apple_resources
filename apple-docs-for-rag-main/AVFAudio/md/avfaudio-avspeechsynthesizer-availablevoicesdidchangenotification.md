

- AVFAudio
- AVSpeechSynthesizer
-  availableVoicesDidChangeNotification 

Type Property

# availableVoicesDidChangeNotification

A notification that indicates a change in available voices for speech synthesis.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class let availableVoicesDidChangeNotification: NSNotification.Name
```

## Discussion

The system posts this notification when available voices for speech synthesis on the system change. For example, a new personal voice becomes available and the user authorized the app to access personal voices. Or new 3rd party voices become available through an app the user downloads.

## See Also

### Enabling personal voices

class var personalVoiceAuthorizationStatus: AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus

Your app’s authorization to use personal voices.

class func requestPersonalVoiceAuthorization(completionHandler: (AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus) -> Void)

Prompts the user to authorize your app to use personal voices.

enum PersonalVoiceAuthorizationStatus

An enumeration that models the personal voices authorization status.




- AVFAudio
- AVSpeechSynthesizer
-  requestPersonalVoiceAuthorization(completionHandler:) 

Type Method

# requestPersonalVoiceAuthorization(completionHandler:)

Prompts the user to authorize your app to use personal voices.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class func requestPersonalVoiceAuthorization(completionHandler handler: @escaping (AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus) -> Void)
```

``` source
class func requestPersonalVoiceAuthorization() async -> AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus
```

## Parameters 

`handler`  

A completion handler that the system calls after the user responds to a request to authorize use of personal voices, which receives the authorization status as an argument.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func requestPersonalVoiceAuthorization() async -> AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Enabling personal voices

class var personalVoiceAuthorizationStatus: AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus

Your app’s authorization to use personal voices.

class let availableVoicesDidChangeNotification: NSNotification.Name

A notification that indicates a change in available voices for speech synthesis.

enum PersonalVoiceAuthorizationStatus

An enumeration that models the personal voices authorization status.


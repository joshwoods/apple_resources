

- AVFAudio
- AVAudioApplication
-  requestMicrophoneInjectionPermission(completionHandler:) 

Type Method

# requestMicrophoneInjectionPermission(completionHandler:)

Requests the app’s permission to add audio to calls.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.2+

``` source
class func requestMicrophoneInjectionPermission(completionHandler response: @escaping (AVAudioApplication.MicrophoneInjectionPermission) -> Void)
```

``` source
class func requestMicrophoneInjectionPermission() async -> AVAudioApplication.MicrophoneInjectionPermission
```

## Discussion

The system immediately returns a response if a person has already granted or denied the app permission, or if the service is in a disabled state. Otherwise, it presents a dialog to request permission and returns a result when a person dismisses the UI.

## See Also

### Requesting microphone injection permission

var microphoneInjectionPermission: AVAudioApplication.MicrophoneInjectionPermission

A value that indicates an app’s permission to add audio to calls.

enum MicrophoneInjectionPermission

Constants that indicate an app’s permission to add audio to calls.


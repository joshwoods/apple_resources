

- AVFAudio
- AVAudioApplication
-  microphoneInjectionPermission 

Instance Property

# microphoneInjectionPermission

A value that indicates an app’s permission to add audio to calls.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.2+

``` source
var microphoneInjectionPermission: AVAudioApplication.MicrophoneInjectionPermission { get }
```

## See Also

### Requesting microphone injection permission

class func requestMicrophoneInjectionPermission(completionHandler: (AVAudioApplication.MicrophoneInjectionPermission) -> Void)

Requests the app’s permission to add audio to calls.

enum MicrophoneInjectionPermission

Constants that indicate an app’s permission to add audio to calls.


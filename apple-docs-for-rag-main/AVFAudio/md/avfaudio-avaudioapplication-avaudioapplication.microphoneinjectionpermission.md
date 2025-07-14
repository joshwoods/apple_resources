

- AVFAudio
- AVAudioApplication
-  AVAudioApplication.MicrophoneInjectionPermission 

Enumeration

# AVAudioApplication.MicrophoneInjectionPermission

Constants that indicate an app’s permission to add audio to calls.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MicrophoneInjectionPermission
```

## Topics

### Permissions

case serviceDisabled

A person disables this service for all apps.

case undetermined

The app hasn’t requested a person’s permission to add audio to calls.

case granted

A person grants the app permission to add audio to calls.

case denied

A person denies the app permission to add audio to calls.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Requesting microphone injection permission

class func requestMicrophoneInjectionPermission(completionHandler: (AVAudioApplication.MicrophoneInjectionPermission) -> Void)

Requests the app’s permission to add audio to calls.

var microphoneInjectionPermission: AVAudioApplication.MicrophoneInjectionPermission

A value that indicates an app’s permission to add audio to calls.


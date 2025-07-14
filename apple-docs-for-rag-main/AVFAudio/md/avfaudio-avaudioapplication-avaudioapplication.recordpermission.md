

- AVFAudio
- AVAudioApplication
-  AVAudioApplication.recordPermission 

Enumeration

# AVAudioApplication.recordPermission

Constants that indicate the app’s permission to record audio.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum recordPermission
```

## Topics

### Permissions

case undetermined

Indicates the app hasn’t requested recording permission.

case granted

Indicates the user grants the app permission to record audio.

case denied

Indicates the user denies the app permission to record audio.

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

### Requesting audio recording permission

class func requestRecordPermission(completionHandler: (Bool) -> Void)

Determines whether the app has permission to record audio.

var recordPermission: AVAudioApplication.recordPermission

The app’s permission to record audio.


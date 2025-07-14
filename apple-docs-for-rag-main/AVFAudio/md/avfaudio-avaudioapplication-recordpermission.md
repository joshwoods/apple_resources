

- AVFAudio
- AVAudioApplication
-  recordPermission 

Instance Property

# recordPermission

The app’s permission to record audio.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var recordPermission: AVAudioApplication.recordPermission { get }
```

## Discussion

See requestRecordPermission(completionHandler:) for more information.

## See Also

### Requesting audio recording permission

class func requestRecordPermission(completionHandler: (Bool) -> Void)

Determines whether the app has permission to record audio.

enum recordPermission

Constants that indicate the app’s permission to record audio.


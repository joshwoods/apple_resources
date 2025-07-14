

- AVFAudio
- AVAudioSession
-  recordPermission Deprecated

Instance Property

# recordPermission

The current recording permission status.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.0–10.0Deprecated

``` source
var recordPermission: AVAudioSession.RecordPermission { get }
```

Deprecated

Use recordPermission on AVAudioApplication instead.

## Return Value

Returns one of three status values:

## Discussion

- The user granted permission to record (AVAudioSession.RecordPermission.granted).

- The user denied recording permission (AVAudioSession.RecordPermission.denied).

- Recording permission hasn’t been requested (AVAudioSession.RecordPermission.undetermined).

## Topics

### Data Types

enum RecordPermission

The values that define the current state of the record permission request.

## See Also

### Requesting permission to record

func requestRecordPermission((Bool) -> Void)

Requests the user’s permission to record audio.

Deprecated




- AVFAudio
- AVAudioSession
-  requestRecordPermission(\_:) Deprecated

Instance Method

# requestRecordPermission(\_:)

Requests the user’s permission to record audio.

iOS 7.0–17.0DeprecatediPadOS 7.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.0–10.0Deprecated

``` source
func requestRecordPermission(_ response: @escaping (Bool) -> Void)
```

Deprecated

Use requestRecordPermission(completionHandler:) on AVAudioApplication instead.

## Parameters 

`response`  

A block, of type `PermissionBlock`, whose sole parameter contains a Boolean value indicating whether the user granted or denied permission to record.

When you call this method, if the user previously granted or denied recording permission, the block executes immediately without displaying a recording permission alert. If the user hasn’t yet granted or denied permission when you call this method, the system displays a recording permission alert and executes the block after the user responds to it.

## Discussion

Recording audio requires explicit permission from the user. The first time your app’s audio session attempts to record from an audio input, the system automatically prompts the user for permission. You can explicitly ask earlier by calling this method. Until the user grants your app permission to record, your app records only silence. When a user responds to a recording permission prompt for your app, the system remembers the choice. If the user has denied recording permission, they can reenable it in Settings \> Privacy \> Microphone.

This method returns immediately, but the `response` block waits for user input if the user hasn’t previously granted or denied recording permission.

The framework may call the thread from a different thread context. Dispatch back to the main thread for any changes that update the user interface.

```
// Request permission to record.
AVAudioSession.sharedInstance().requestRecordPermission { granted in
    if granted {
        // The user granted access. Present recording interface.
    } else {
        // Present message to user indicating that recording
        // can't be performed until they change their preference
        // under Settings -> Privacy -> Microphone
    }
}
```

Important

Apps that access any of the device’s microphones must declare their intent to do so. You do this by including the `NSMicrophoneUsageDescription` key and a corresponding purpose string in your app’s `Info.plist`. When the system prompts the user to allow access, it displays the purpose string as part of the alert.

If an application attempts to access any of the device’s microphones without a corresponding purpose string, the app exits.

## See Also

### Requesting permission to record

var recordPermission: AVAudioSession.RecordPermission

The current recording permission status.

Deprecated


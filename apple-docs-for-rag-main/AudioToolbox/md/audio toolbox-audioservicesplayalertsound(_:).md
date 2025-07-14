

- Audio Toolbox
-  AudioServicesPlayAlertSound(\_:) 

Function

# AudioServicesPlayAlertSound(\_:)

Plays a system sound as an alert.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesPlayAlertSound(_ inSystemSoundID: SystemSoundID)
```

## Parameters 

`inSystemSoundID`  

The system sound object to play as an alert.

Before using this function, call the AudioServicesCreateSystemSoundID(_:_:) function to obtain a system sound.

## Discussion

Depending on the particular iOS device, this function plays a short sound and may invoke vibration. Calling this function does the following on various iOS devices:

- *iPhone*—plays the specified sound. If the user has configured the Settings application for vibration on ring, also invokes vibration. However, the device does *not* vibrate if your app’s audio session is configured with the playAndRecord or record audio session category. This ensures that vibration doesn’t interfere with audio recording. For an explanation of audio session categories, see Categories Express Audio Roles.

- *iPod touch, original*—plays a short alert melody.

- *iPod touch, 2nd generation and newer*—plays the specified sound.

In iOS, the duration of the sound to be played must not be more than 30 seconds.

Note

System-supplied alert sounds and system-supplied user-interface sound effects are not available to your iOS application. For example, using the `kSystemSoundID_UserPreferredAlert` constant as a parameter to the `AudioServicesPlayAlertSound` function will not play anything.

In macOS, when a user has configured System Preferences to flash the screen for alerts, or if sound cannot be rendered, calling this function will result in the screen flashing. In macOS, pass the constant `kSystemSoundID_UserPreferredAlert` to play the alert sound selected by the user in System Preferences. In iOS there is no preferred user alert sound.

To play a short sound not used as an alert, use AudioServicesPlaySystemSound(_:).

## See Also

### Related Documentation

func AudioServicesCreateSystemSoundID(CFURL, UnsafeMutablePointer&lt;SystemSoundID>) -> OSStatus

Creates a system sound object.

### Playing Sounds

func AudioServicesPlayAlertSoundWithCompletion(SystemSoundID, (() -> Void)?)

func AudioServicesPlaySystemSoundWithCompletion(SystemSoundID, (() -> Void)?)

func AudioServicesPlaySystemSound(SystemSoundID)

Plays a system sound object.




- AVFAudio
- AVAudioSession
-  setActive(\_:options:) 

Instance Method

# setActive(\_:options:)

Activates or deactivates your app’s audio session using the specified options.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setActive(
    _ active: Bool,
    options: AVAudioSession.SetActiveOptions = []
) throws
```

## Parameters 

`active`  

Specify true to activate your app’s audio session, or false to deactivate it.

`options`  

An integer bit mask containing one or more constants from the AVAudioSession.SetActiveOptions enumeration.

## Discussion

Your app may activate a session with category playback when another app is hosting a call, for example to start a `SharePlay` activity. However, your app isn’t permitted to capture the microphone of the active call.

Note

If you attempt to activate a session with category record or playAndRecord when another app is already hosting a call, then your session fails with the error AVAudioSessionErrorInsufficientPriority.

The session fails to activate if another audio session has higher priority than yours (such as a phone call) and neither audio session allows mixing. Deactivating an audio session with running audio objects stops the objects, makes the session inactive, and returns an AVAudioSessionErrorCodeIsBusy error.

When your app deactivates a session, the return value is false but the active state changes to deactivate.

## Topics

### Data Types

struct SetActiveOptions

Options that provide additional information about your app’s audio intentions upon session deactivation.

## See Also

### Activating the audio configuration

func activate(options: AVAudioSessionActivationOptions, completionHandler: (Bool, (any Error)?) -> Void)

Activates an audio session asynchronously on watchOS.

struct AVAudioSessionActivationOptions

Constants that describe the options to pass when activating the audio session.


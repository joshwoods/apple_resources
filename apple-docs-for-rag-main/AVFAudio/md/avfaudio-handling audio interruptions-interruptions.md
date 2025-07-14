

- AVFAudio
-  Handling audio interruptions 

Article

# Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

## Overview

Interruptions are a common part of the iOS and watchOS user experiences. For example, consider the scenario of receiving a phone call while you’re watching a movie in the TV app on your iPhone. In this case, the movie’s audio fades out, playback pauses, and the sound of the call’s ringtone fades in. If you decline the call, control returns to the TV app, and playback begins again as the movie’s audio fades in.

At the center of this behavior is your app’s audio session. As interruptions begin and end, the audio session notifies any registered observers so they can take appropriate action. For example, AVPlayer monitors your app’s audio session and automatically pauses playback in response to interruption events. You can monitor these changes by key-value observing the player’s timeControlStatus property, and update your user interface as necessary when the player pauses and resumes playback.

### Customize the interruption behavior

Most apps rely on the system’s default interruption behavior. However, AVAudioSession provides ways to customize the default behavior to better accommodate your app’s needs:

- Recent iPad models provide a feature that mutes the built-in microphone at the hardware level when the user closes the device’s Smart Folio cover. If your app plays and records audio, you may want to continue playback even if the system mutes the microphone. You can disable the default interruption behavior by setting the overrideMutedMicrophoneInterruption option when configuring your audio session.

- System alerts, such as receiving an incoming phone call, interrupt the active audio session. If you prefer that the system not interrupt your app’s audio session in these cases, you can indicate this preference by setting a value for the setPrefersNoInterruptionsFromSystemAlerts(_:) method.

### Observe audio session interruptions

You can directly observe interruption notifications that AVAudioSession posts. This might be useful if you want to know when the system pauses playback due to an interruption or another reason, such as a route change. To observe audio interruptions, begin by registering to observe notifications of type interruptionNotification.

```
func setupNotifications() {
    // Get the default notification center instance.
    let nc = NotificationCenter.default
    nc.addObserver(self,
                   selector: #selector(handleInterruption),
                   name: AVAudioSession.interruptionNotification,
                   object: AVAudioSession.sharedInstance())
}

@objc func handleInterruption(notification: Notification) {
    // To implement.
}
```

### Handle audio session interruptions

The posted Notification object contains a populated user-information dictionary that provides the details of the interruption. You determine the type of interruption by retrieving the AVAudioSession.InterruptionType value from the userInfo dictionary. The interruption type indicates whether the interruption is beginning or ending.

```
@objc func handleInterruption(notification: Notification) {
    guard let userInfo = notification.userInfo,
        let typeValue = userInfo[AVAudioSessionInterruptionTypeKey] as? UInt,
        let type = AVAudioSession.InterruptionType(rawValue: typeValue) else {
            return
    }

    // Switch over the interruption type.
    switch type {

    case .began:
        // An interruption began. Update the UI as necessary.

    case .ended:
       // An interruption ended. Resume playback, if appropriate.

        guard let optionsValue = userInfo[AVAudioSessionInterruptionOptionKey] as? UInt else { return }
        let options = AVAudioSession.InterruptionOptions(rawValue: optionsValue)
        if options.contains(.shouldResume) {
            // An interruption ended. Resume playback.
        } else {
            // An interruption ended. Don't resume playback.
        }

    default: ()
    }
}
```

If the interruption type is AVAudioSession.InterruptionType.ended, the userInfo dictionary contains an AVAudioSession.InterruptionOptions value, which you use to determine whether playback automatically resumes.

## See Also

### System audio

Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Adding synthesized speech to calls

Provide a more accessible experience by adding your app’s audio to a call.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

class AVAudioSession

An object that communicates to the system how you intend to use audio in your app.

class AVAudioApplication

An object that manages one or more audio sessions that belong to an app.

class AVAudioRoutingArbiter

An object for configuring macOS apps to participate in AirPods Automatic Switching.


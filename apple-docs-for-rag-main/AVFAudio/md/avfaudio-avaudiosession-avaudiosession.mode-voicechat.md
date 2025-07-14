

- AVFAudio
- AVAudioSession
- AVAudioSession.Mode
-  voiceChat 

Type Property

# voiceChat

A mode that indicates that your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let voiceChat: AVAudioSession.Mode
```

## Discussion

Use this mode for Voice over IP (VoIP) apps that use the playAndRecord category. When you set this mode, the session optimizes the device’s tonal equalization for voice and reduces the set of allowable audio routes to only those appropriate for voice chat.

Using this mode has the side effect of enabling the allowBluetooth category option.

For apps that use voice or video chat, also use the Voice-Processing I/O audio unit. The Voice-Processing I/O unit provides several features for VoIP apps, including automatic gain correction, adjustment of voice processing, and muting. See Voice-Processing I/O Unit for more information.

If an app uses the Voice-Processing I/O audio unit and hasn’t set its mode to one of the chat modes (voice, video, or game), the session sets the voiceChat mode implicitly. On the other hand, if the app had previously set its category to playAndRecord and its mode to videoChat or gameChat, instantiating the Voice-Processing I/O audio unit doesn’t cause the mode to change.

## See Also

### Getting Standard Session Modes

static let `default`: AVAudioSession.Mode

The default audio session mode.

static let gameChat: AVAudioSession.Mode

A mode that the GameKit framework sets on behalf of an application that uses GameKit’s voice chat service.

static let measurement: AVAudioSession.Mode

A mode that indicates that your app is performing measurement of audio input or output.

static let moviePlayback: AVAudioSession.Mode

A mode that indicates that your app is playing back movie content.

static let spokenAudio: AVAudioSession.Mode

A mode used for continuous spoken audio to pause the audio when another app plays a short audio prompt.

static let videoChat: AVAudioSession.Mode

A mode that indicates that your app is engaging in online video conferencing.

static let videoRecording: AVAudioSession.Mode

A mode that indicates that your app is recording a movie.

static let voicePrompt: AVAudioSession.Mode

A mode that indicates that your app plays audio using text-to-speech.


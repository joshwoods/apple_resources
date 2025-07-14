

- AVFAudio
- AVAudioSession
- AVAudioSession.Mode
-  measurement 

Type Property

# measurement

A mode that indicates that your app is performing measurement of audio input or output.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let measurement: AVAudioSession.Mode
```

## Discussion

Use this mode for apps that need to minimize the amount of system-supplied signal processing to input and output signals. If recording on devices with more than one built-in microphone, the session uses the primary microphone.

For use with the playback, record, or playAndRecord audio session categories.

Important

This mode disables some dynamics processing on input and output signals, resulting in a lower-output playback level.

## See Also

### Getting Standard Session Modes

static let `default`: AVAudioSession.Mode

The default audio session mode.

static let gameChat: AVAudioSession.Mode

A mode that the GameKit framework sets on behalf of an application that uses GameKit’s voice chat service.

static let moviePlayback: AVAudioSession.Mode

A mode that indicates that your app is playing back movie content.

static let spokenAudio: AVAudioSession.Mode

A mode used for continuous spoken audio to pause the audio when another app plays a short audio prompt.

static let videoChat: AVAudioSession.Mode

A mode that indicates that your app is engaging in online video conferencing.

static let videoRecording: AVAudioSession.Mode

A mode that indicates that your app is recording a movie.

static let voiceChat: AVAudioSession.Mode

A mode that indicates that your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

static let voicePrompt: AVAudioSession.Mode

A mode that indicates that your app plays audio using text-to-speech.


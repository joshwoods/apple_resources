

- AVFAudio
- AVAudioSession
- AVAudioSession.Mode
-  spokenAudio 

Type Property

# spokenAudio

A mode used for continuous spoken audio to pause the audio when another app plays a short audio prompt.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let spokenAudio: AVAudioSession.Mode
```

## Discussion

This mode is appropriate for apps that play continuous spoken audio, such as podcasts or audio books. Setting this mode indicates that your app should pause, rather than duck, its audio if another app plays a spoken audio prompt. After the interrupting app’s audio ends, you can resume your app’s audio playback.

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

static let videoChat: AVAudioSession.Mode

A mode that indicates that your app is engaging in online video conferencing.

static let videoRecording: AVAudioSession.Mode

A mode that indicates that your app is recording a movie.

static let voiceChat: AVAudioSession.Mode

A mode that indicates that your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

static let voicePrompt: AVAudioSession.Mode

A mode that indicates that your app plays audio using text-to-speech.


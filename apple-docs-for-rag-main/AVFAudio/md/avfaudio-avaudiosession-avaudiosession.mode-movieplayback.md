

- AVFAudio
- AVAudioSession
- AVAudioSession.Mode
-  moviePlayback 

Type Property

# moviePlayback

A mode that indicates that your app is playing back movie content.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let moviePlayback: AVAudioSession.Mode
```

## Discussion

When you set this mode, the audio session uses signal processing to enhance movie playback for certain audio routes such as built-in speaker or headphones. You may only use this mode with the playback audio session category.

## See Also

### Getting Standard Session Modes

static let `default`: AVAudioSession.Mode

The default audio session mode.

static let gameChat: AVAudioSession.Mode

A mode that the GameKit framework sets on behalf of an application that uses GameKit’s voice chat service.

static let measurement: AVAudioSession.Mode

A mode that indicates that your app is performing measurement of audio input or output.

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


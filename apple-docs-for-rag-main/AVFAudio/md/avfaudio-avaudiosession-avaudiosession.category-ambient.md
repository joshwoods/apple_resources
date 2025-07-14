

- AVFAudio
- AVAudioSession
- AVAudioSession.Category
-  ambient 

Type Property

# ambient

The category for an app in which sound playback is nonprimary — that is, your app also works with the sound turned off.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let ambient: AVAudioSession.Category
```

## Discussion

This category is also appropriate for “play-along” apps, such as a virtual piano that a user plays while the Music app is playing. When you use this category, audio from other apps mixes with your audio. Screen locking and the Silent switch (on iPhone, the Ring/Silent switch) silence your audio.

## See Also

### Getting Standard Categories

static let multiRoute: AVAudioSession.Category

The category for routing distinct streams of audio data to different output devices at the same time.

static let playAndRecord: AVAudioSession.Category

The category for recording (input) and playback (output) of audio, such as for a Voice over Internet Protocol (VoIP) app.

static let playback: AVAudioSession.Category

The category for playing recorded music or other sounds that are central to the successful use of your app.

static let record: AVAudioSession.Category

The category for recording audio while also silencing playback audio.

static let soloAmbient: AVAudioSession.Category

The default audio session category.

static let audioProcessing: AVAudioSession.Category

The category for using an audio hardware codec or signal processor while not playing or recording audio.

Deprecated




- AVFAudio
- AVAudioSession
- AVAudioSession.Category
-  soloAmbient 

Type Property

# soloAmbient

The default audio session category.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let soloAmbient: AVAudioSession.Category
```

## Discussion

Your audio is silenced by screen locking and by the Silent switch (called the *Ring/Silent switch* on iPhone).

By default, using this category implies that your app’s audio is nonmixable—activating your session will interrupt any other audio sessions which are also nonmixable. To allow mixing, use the ambient category instead.

## See Also

### Getting Standard Categories

static let ambient: AVAudioSession.Category

The category for an app in which sound playback is nonprimary — that is, your app also works with the sound turned off.

static let multiRoute: AVAudioSession.Category

The category for routing distinct streams of audio data to different output devices at the same time.

static let playAndRecord: AVAudioSession.Category

The category for recording (input) and playback (output) of audio, such as for a Voice over Internet Protocol (VoIP) app.

static let playback: AVAudioSession.Category

The category for playing recorded music or other sounds that are central to the successful use of your app.

static let record: AVAudioSession.Category

The category for recording audio while also silencing playback audio.

static let audioProcessing: AVAudioSession.Category

The category for using an audio hardware codec or signal processor while not playing or recording audio.

Deprecated


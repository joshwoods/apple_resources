

- AVFAudio
- AVAudioSession
- AVAudioSession.Category
-  multiRoute 

Type Property

# multiRoute

The category for routing distinct streams of audio data to different output devices at the same time.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let multiRoute: AVAudioSession.Category
```

## Discussion

This category can be used for input, output, or both. For example, use this category to route audio to both a USB device and a set of headphones. Use of this category requires a more detailed knowledge of, and interaction with, the capabilities of the available audio routes.

Important

Route changes can invalidate part or all of your multi-route configuration. When using the multiRoute category, it is essential that you register to observe routeChangeNotification notifications and update your configuration as necessary.

## See Also

### Getting Standard Categories

static let ambient: AVAudioSession.Category

The category for an app in which sound playback is nonprimary — that is, your app also works with the sound turned off.

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


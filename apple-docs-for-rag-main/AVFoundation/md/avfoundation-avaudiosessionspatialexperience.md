

- AVFoundation
-  AVAudioSessionSpatialExperience 

Protocol

# AVAudioSessionSpatialExperience

A protocol that defines types of spatial audio experiences that the system supports.

visionOS 1.0+

``` source
protocol AVAudioSessionSpatialExperience
```

## Topics

### Specifying the experience

static func fixed(soundStageSize: AVAudioSession.SoundStageSize) -> Self

Returns a fixed spatial experience configured for the specified sound stage size.

static func headTracked(soundStageSize: AVAudioSession.SoundStageSize, anchoringStrategy: AVAudioSession.AnchoringStrategy) -> Self

Returns a head-tracked spatial experience configured for the specified sound stage size and anchoring strategy.

enum SoundStageSize

Constants that specify the perceived size of sounds the audio session plays.

enum AnchoringStrategy

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

static var bypassed: AVAudioSession.BypassedSpatialExperience

A nonspatial experience.

## See Also

### System audio

Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

class AVAudioSession

An object that communicates to the system how you intend to use audio in your app.

class AVAudioApplication

An object that manages one or more audio sessions that belong to an app.

class AVAudioRoutingArbiter

An object for configuring macOS apps to participate in AirPods Automatic Switching.


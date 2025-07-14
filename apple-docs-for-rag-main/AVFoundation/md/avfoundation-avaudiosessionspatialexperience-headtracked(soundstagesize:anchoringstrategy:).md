

- AVFoundation
- AVAudioSessionSpatialExperience
-  headTracked(soundStageSize:anchoringStrategy:) 

Type Method

# headTracked(soundStageSize:anchoringStrategy:)

Returns a head-tracked spatial experience configured for the specified sound stage size and anchoring strategy.

visionOS 1.0+

``` source
static func headTracked(
    soundStageSize: AVAudioSession.SoundStageSize,
    anchoringStrategy: AVAudioSession.AnchoringStrategy
) -> Self
```

Available when `Self` is `AVAudioSession.HeadTrackedSpatialExperience`.

## Parameters 

`soundStageSize`  

The size of the sound stage.

`anchoringStrategy`  

The anchoring strategy the experience uses.

## Return Value

A new spatial experience.

## See Also

### Specifying the experience

static func fixed(soundStageSize: AVAudioSession.SoundStageSize) -> Self

Returns a fixed spatial experience configured for the specified sound stage size.

enum SoundStageSize

Constants that specify the perceived size of sounds the audio session plays.

enum AnchoringStrategy

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

static var bypassed: AVAudioSession.BypassedSpatialExperience

A nonspatial experience.


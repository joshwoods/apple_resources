

- AVFAudio
- AVAudio3DMixingRenderingAlgorithm
-  AVAudio3DMixingRenderingAlgorithm.auto 

Case

# AVAudio3DMixingRenderingAlgorithm.auto

Automatically selects the highest-quality rendering algorithm available for the current playback hardware.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case auto
```

## Discussion

This selects the highest-quality rendering algorithm available for the current playback hardware.

The algorithm may not be identical to other existing algorithms. It may change in the future as new algorithms emerge.

When in manual rendering mode or wired output, you may need to set the outputType on AVAudioEnvironmentNode. Multichannel rendering requires setting a channel layout on an AVAudioEnvironmentNode output.

## See Also

### Rendering Algorithms

case equalPowerPanning

An algorithm that pans the data of the mixer bus into a stereo field.

case HRTF

A high-quality algorithm that uses filtering to emulate 3D space in headphones.

case HRTFHQ

A higher-quality head-related transfer function rendering algorithm.

case soundField

An algorithm that renders to multichannel hardware.

case sphericalHead

An algorithm that emulates 3D space in headphones by simulating interaural time delays and other spatial cues.

case stereoPassThrough

An algorithm to use when the source data doesn’t need localization.


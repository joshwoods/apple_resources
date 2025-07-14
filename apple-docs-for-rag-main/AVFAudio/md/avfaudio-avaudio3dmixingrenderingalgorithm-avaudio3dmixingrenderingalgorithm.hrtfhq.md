

- AVFAudio
- AVAudio3DMixingRenderingAlgorithm
-  AVAudio3DMixingRenderingAlgorithm.HRTFHQ 

Case

# AVAudio3DMixingRenderingAlgorithm.HRTFHQ

A higher-quality head-related transfer function rendering algorithm.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
case HRTFHQ
```

## Discussion

In comparison to AVAudio3DMixingRenderingAlgorithm.HRTF, this option’s improvements focus on the frequency response and localization of sources in 3D space.

## See Also

### Rendering Algorithms

case auto

Automatically selects the highest-quality rendering algorithm available for the current playback hardware.

case equalPowerPanning

An algorithm that pans the data of the mixer bus into a stereo field.

case HRTF

A high-quality algorithm that uses filtering to emulate 3D space in headphones.

case soundField

An algorithm that renders to multichannel hardware.

case sphericalHead

An algorithm that emulates 3D space in headphones by simulating interaural time delays and other spatial cues.

case stereoPassThrough

An algorithm to use when the source data doesn’t need localization.


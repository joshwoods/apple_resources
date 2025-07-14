

- AVFAudio
- AVAudio3DMixingRenderingAlgorithm
-  AVAudio3DMixingRenderingAlgorithm.sphericalHead 

Case

# AVAudio3DMixingRenderingAlgorithm.sphericalHead

An algorithm that emulates 3D space in headphones by simulating interaural time delays and other spatial cues.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
case sphericalHead
```

## Discussion

This is slightly less CPU-intensive than AVAudio3DMixingRenderingAlgorithm.HRTF.

## See Also

### Rendering Algorithms

case auto

Automatically selects the highest-quality rendering algorithm available for the current playback hardware.

case equalPowerPanning

An algorithm that pans the data of the mixer bus into a stereo field.

case HRTF

A high-quality algorithm that uses filtering to emulate 3D space in headphones.

case HRTFHQ

A higher-quality head-related transfer function rendering algorithm.

case soundField

An algorithm that renders to multichannel hardware.

case stereoPassThrough

An algorithm to use when the source data doesn’t need localization.


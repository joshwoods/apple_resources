

- AVFAudio
- AVAudio3DMixingRenderingAlgorithm
-  AVAudio3DMixingRenderingAlgorithm.soundField 

Case

# AVAudio3DMixingRenderingAlgorithm.soundField

An algorithm that renders to multichannel hardware.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
case soundField
```

## Discussion

This takes data the system renders with AVAudio3DMixingRenderingAlgorithm.soundField and distributes it among all of the output channels with a weighting toward the location of the sound. This algorithm is very effective for ambient sounds. Those sounds may derive from a specific location, but they fill the listener’s entire space.

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

case sphericalHead

An algorithm that emulates 3D space in headphones by simulating interaural time delays and other spatial cues.

case stereoPassThrough

An algorithm to use when the source data doesn’t need localization.


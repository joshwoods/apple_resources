

- AVFAudio
- AVAudio3DMixingRenderingAlgorithm
-  AVAudio3DMixingRenderingAlgorithm.stereoPassThrough 

Case

# AVAudio3DMixingRenderingAlgorithm.stereoPassThrough

An algorithm to use when the source data doesn’t need localization.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
case stereoPassThrough
```

## Discussion

This takes mono and stereo input and passes it to channels 1 and 2 without localization. If the input and output `AudioChannelLayout` differ, mixing happens according to the kAudioFormatProperty_MatrixMixMap property of the layouts.

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

case sphericalHead

An algorithm that emulates 3D space in headphones by simulating interaural time delays and other spatial cues.


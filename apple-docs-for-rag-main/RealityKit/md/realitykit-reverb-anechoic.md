

- RealityKit
- Reverb
-  anechoic 

Type Property

# anechoic

A reverb instance that applies no reverberation to spatial audio sources.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static let anechoic: Reverb
```

## Discussion

Warning

anechoic will cause spatial audio sources to lose externalization, or the sense that an audio source is in a person’s space. Only use this case when when the immersive environment is abstract or otherwise unrealistic.


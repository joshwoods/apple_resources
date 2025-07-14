

- AVFAudio
- AVAudioUnitReverb
-  wetDryMix 

Instance Property

# wetDryMix

The blend of the wet and dry signals.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var wetDryMix: Float { get set }
```

## Discussion

You specify the blend as a percentage. The range is `0%` through `100%`, where `0%` represents all dry.




- AVFAudio
- AVAudioStereoMixing
-  pan 

Instance Property

# pan

The bus’s stereo pan.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var pan: Float { get set }
```

**Required**

## Discussion

The default value is `0.0`, and the range of valid values is `-1.0` to `1.0`. Only the AVAudioEnvironmentNode class implements this property.


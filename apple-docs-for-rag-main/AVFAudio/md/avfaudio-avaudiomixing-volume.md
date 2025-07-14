

- AVFAudio
- AVAudioMixing
-  volume 

Instance Property

# volume

The bus’s input volume.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var volume: Float { get set }
```

**Required**

## Discussion

The default value is `1.0`, and the range of valid values is `0.0` to `1.0`. Only the AVAudioEnvironmentNode and the AVAudioMixerNode implement this property.


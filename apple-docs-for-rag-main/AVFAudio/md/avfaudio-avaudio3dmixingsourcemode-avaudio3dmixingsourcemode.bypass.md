

- AVFAudio
- AVAudio3DMixingSourceMode
-  AVAudio3DMixingSourceMode.bypass 

Case

# AVAudio3DMixingSourceMode.bypass

A mode that does no spatial rendering.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case bypass
```

## Discussion

If input and output audio channel layouts are equivalent, the framework copies all input channels directly to corresponding output channels. If the input and output audio channel layouts differ, the framework mixes according to the kAudioFormatProperty_MatrixMixMap property of the layouts. It applies no occlusion, obstruction, or reverb in this mode.

## See Also

### Source Modes

case spatializeIfMono

A mono input bus that renders as a point source at the location of the source node.

case pointSource

All channels of the bus render as a single source at the location of the source node.

case ambienceBed

The input channels spread around the listener as far-field sources that anchor to global space.


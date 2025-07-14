

- AVFAudio
- AVAudio3DMixingSourceMode
-  AVAudio3DMixingSourceMode.ambienceBed 

Case

# AVAudio3DMixingSourceMode.ambienceBed

The input channels spread around the listener as far-field sources that anchor to global space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case ambienceBed
```

## Discussion

The rendering depends on listener orientation, but not on listener position. The audio channel layout of the bus specifies the directions of the input channels. The direction of the source node controls the rotation of the bed in the global space.

## See Also

### Source Modes

case spatializeIfMono

A mono input bus that renders as a point source at the location of the source node.

case bypass

A mode that does no spatial rendering.

case pointSource

All channels of the bus render as a single source at the location of the source node.


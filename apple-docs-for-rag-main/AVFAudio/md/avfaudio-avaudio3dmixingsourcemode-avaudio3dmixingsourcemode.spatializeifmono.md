

- AVFAudio
- AVAudio3DMixingSourceMode
-  AVAudio3DMixingSourceMode.spatializeIfMono 

Case

# AVAudio3DMixingSourceMode.spatializeIfMono

A mono input bus that renders as a point source at the location of the source node.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case spatializeIfMono
```

## Discussion

The system bypasses an input bus with more than one channel. This is equivalent to AVAudio3DMixingSourceMode.pointSource for a mono bus and AVAudio3DMixingSourceMode.bypass for a bus with more than one channel.

## See Also

### Source Modes

case bypass

A mode that does no spatial rendering.

case pointSource

All channels of the bus render as a single source at the location of the source node.

case ambienceBed

The input channels spread around the listener as far-field sources that anchor to global space.


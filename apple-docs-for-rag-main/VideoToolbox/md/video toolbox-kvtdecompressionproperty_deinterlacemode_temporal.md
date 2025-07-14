

- Video Toolbox
-  kVTDecompressionProperty_DeinterlaceMode_Temporal 

Global Variable

# kVTDecompressionProperty_DeinterlaceMode_Temporal

A temporal deinterlace mode.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionProperty_DeinterlaceMode_Temporal: CFString
```

## Discussion

Applies a filter that uses a window of multiple frames to generate deinterlaced results, and provides a better result at the expense of a pipeline delay.

This mode is only used if kVTDecodeFrame_EnableTemporalProcessing is set, otherwise a non-temporal mode will be used instead.

## See Also

### Deinterlace Modes

let kVTDecompressionProperty_DeinterlaceMode_VerticalFilter: CFString

A vertical filter deinterlace mode.




- Video Toolbox
-  kVTDecompressionPropertyKey_ThreadCount 

Global Variable

# kVTDecompressionPropertyKey_ThreadCount

The number of threads used by a codec or the suggested number of threads to use (optional).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_ThreadCount: CFString
```

## Discussion

This is an optional property for video decoders to implement.

## See Also

### Decoder Behavior

let kVTDecompressionPropertyKey_RealTime: CFString

A Boolean value indicating whether it’s recommended that the video decoder perform decompression in real time.

let kVTDecompressionPropertyKey_MaximizePowerEfficiency: CFString

let kVTDecompressionPropertyKey_FieldMode: CFString

Modes for special handling of interlaced content (optional).

let kVTDecompressionPropertyKey_DeinterlaceMode: CFString

Modes for requesting a specific deinterlacing technique.

let kVTDecompressionPropertyKey_ReducedResolutionDecode: CFString

Request decoding at smaller resolutions than full-size (optional).

let kVTDecompressionPropertyKey_ReducedCoefficientDecode: CFString

Requests approximation during decoding.

let kVTDecompressionPropertyKey_ReducedFrameDelivery: CFString

The proportion of frames that should be delivered, indicating that the rest may be dropped.

let kVTDecompressionPropertyKey_OnlyTheseFrames: CFString

Requests that frames be filtered by type.

let kVTDecompressionProperty_TemporalLevelLimit: CFString

let kVTDecompressionPropertyKey_SuggestedQualityOfServiceTiers: CFString

An array of dictionaries that describe decreasing quality-of-service levels that clients can use to maintain realtime playback (optional).

let kVTDecompressionPropertyKey_SupportedPixelFormatsOrderedByQuality: CFString

An array indicating quality levels among pixel formats.

let kVTDecompressionPropertyKey_SupportedPixelFormatsOrderedByPerformance: CFString

An array indicating speed tradeoffs between pixel formats (optional).

let kVTDecompressionPropertyKey_PixelFormatsWithReducedResolutionSupport: CFString

Pixel formats that support reduced-resolution decoding (optional).

let kVTDecompressionPropertyKey_AllowBitstreamToChangeFrameDimensions: CFString


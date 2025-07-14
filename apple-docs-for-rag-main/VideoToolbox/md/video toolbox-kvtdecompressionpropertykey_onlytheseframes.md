

- Video Toolbox
-  kVTDecompressionPropertyKey_OnlyTheseFrames 

Global Variable

# kVTDecompressionPropertyKey_OnlyTheseFrames

Requests that frames be filtered by type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_OnlyTheseFrames: CFString
```

## Discussion

This is an optional property for video decoders to implement. If supported, it requests that the decoder limit decoding to the frame type specified by one of the `Only These Frames Constants`. This key may be used on its own, or may appear in the dictionaries returned in the array obtained from kVTDecompressionPropertyKey_SuggestedQualityOfServiceTiers.

If kVTDecompressionPropertyKey_ReducedFrameDelivery is supported and used in conjunction with this property, the `ReducedFrameDelivery` is the proportion of the frames selected by this property. For example, a dictionary containing `[{kVTDecompressionPropertyKey_OnlyTheseFrames, kVTDecompressionProperty_OnlyTheseFrames_KeyFrames}, {kVTDecompressionPropertyKey_ReducedFrameDelivery, 0.25}]` would request that the decoder only deliver 1/4 of keyframes.

## Topics

### Frame Constants

let kVTDecompressionProperty_OnlyTheseFrames_AllFrames: CFString

let kVTDecompressionProperty_OnlyTheseFrames_IFrames: CFString

let kVTDecompressionProperty_OnlyTheseFrames_KeyFrames: CFString

let kVTDecompressionProperty_OnlyTheseFrames_NonDroppableFrames: CFString

## See Also

### Decoder Behavior

let kVTDecompressionPropertyKey_RealTime: CFString

A Boolean value indicating whether it’s recommended that the video decoder perform decompression in real time.

let kVTDecompressionPropertyKey_MaximizePowerEfficiency: CFString

let kVTDecompressionPropertyKey_ThreadCount: CFString

The number of threads used by a codec or the suggested number of threads to use (optional).

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




- Video Toolbox
-  kVTDecompressionPropertyKey_SuggestedQualityOfServiceTiers 

Global Variable

# kVTDecompressionPropertyKey_SuggestedQualityOfServiceTiers

An array of dictionaries that describe decreasing quality-of-service levels that clients can use to maintain realtime playback (optional).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_SuggestedQualityOfServiceTiers: CFString
```

## Discussion

This is an optional property for video decoders to implement. This property value is an array of doc://com.apple.documentation/documentation/corefoundation/cfdictionary-rum objects describing different reduced frame delivery options supported by the decoder.

The first dictionary in the array should contain the set of properties that restore the default (full) quality of service; later dictionaries should contain property sets with decreasing qualities of service. Clients can work their way down these tiers until they are able to keep up with the frame rate. The dictionaries can be applied directly on the decompression session using VTSessionSetProperties(_:propertyDictionary:) in order to request that quality of service tier be enforced.

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

let kVTDecompressionPropertyKey_OnlyTheseFrames: CFString

Requests that frames be filtered by type.

let kVTDecompressionProperty_TemporalLevelLimit: CFString

let kVTDecompressionPropertyKey_SupportedPixelFormatsOrderedByQuality: CFString

An array indicating quality levels among pixel formats.

let kVTDecompressionPropertyKey_SupportedPixelFormatsOrderedByPerformance: CFString

An array indicating speed tradeoffs between pixel formats (optional).

let kVTDecompressionPropertyKey_PixelFormatsWithReducedResolutionSupport: CFString

Pixel formats that support reduced-resolution decoding (optional).

let kVTDecompressionPropertyKey_AllowBitstreamToChangeFrameDimensions: CFString


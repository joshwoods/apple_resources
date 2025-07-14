

- Video Toolbox
- VTDecompressionSession
-  Decompression Properties 

API Collection

# Decompression Properties

Properties used to configure a VideoToolbox decompression session.

## Topics

### Pixel Buffer Pools

let kVTDecompressionPropertyKey_PixelBufferPool: CFString

A pixel buffer pool for pixel buffers being output by the decompression session.

let kVTDecompressionPropertyKey_PixelBufferPoolIsShared: CFString

A Boolean value indicating whether a common pixel buffer pool is shared between the video decoder and the session client.

let kVTDecompressionPropertyKey_OutputPoolRequestedMinimumBufferCount: CFString

The requested minimum buffer count that a decompression session should use for its output pixel buffer pool, without releasing buffers while the number in use is below this level.

### Asynchronous State

let kVTDecompressionPropertyKey_NumberOfFramesBeingDecoded: CFString

Returns the number of frames currently being decoded.

let kVTDecompressionPropertyKey_MinOutputPresentationTimeStampOfFramesBeingDecoded: CFString

The minimum output presentation timestamp of the frames currently being decoded.

let kVTDecompressionPropertyKey_MaxOutputPresentationTimeStampOfFramesBeingDecoded: CFString

The maximum output presentation timestamp of the frames currently being decoded.

### Content

let kVTDecompressionPropertyKey_ContentHasInterframeDependencies: CFString

An optional Boolean property indicating if the content being decoded has interframe dependencies, if the decoder knows.

### Hardware Acceleration

let kVTVideoDecoderSpecification_EnableHardwareAcceleratedVideoDecoder: CFString

A Boolean value indicating whether VideoToolbox uses a hardware-accelerated video decoder, if available.

let kVTVideoDecoderSpecification_RequireHardwareAcceleratedVideoDecoder: CFString

A Boolean value indicating whether to require hardware-accelerated decoding.

let kVTDecompressionPropertyKey_UsingHardwareAcceleratedVideoDecoder: CFString

Indicates if a hardware-accelerated video decoder is being used.

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

let kVTDecompressionPropertyKey_SuggestedQualityOfServiceTiers: CFString

An array of dictionaries that describe decreasing quality-of-service levels that clients can use to maintain realtime playback (optional).

let kVTDecompressionPropertyKey_SupportedPixelFormatsOrderedByQuality: CFString

An array indicating quality levels among pixel formats.

let kVTDecompressionPropertyKey_SupportedPixelFormatsOrderedByPerformance: CFString

An array indicating speed tradeoffs between pixel formats (optional).

let kVTDecompressionPropertyKey_PixelFormatsWithReducedResolutionSupport: CFString

Pixel formats that support reduced-resolution decoding (optional).

let kVTDecompressionPropertyKey_AllowBitstreamToChangeFrameDimensions: CFString

### Post-Decompression Processing

let kVTDecompressionPropertyKey_PixelTransferProperties: CFString

Specific pixel transfer features to be used during decompression.

let kVTVideoDecoderSpecification_RequiredDecoderGPURegistryID: CFString

let kVTVideoDecoderSpecification_PreferredDecoderGPURegistryID: CFString

let kVTDecompressionPropertyKey_UsingGPURegistryID: CFString

let kVTDecompressionPropertyKey_PropagatePerFrameHDRDisplayMetadata: CFString

let kVTDecompressionPropertyKey_GeneratePerFrameHDRDisplayMetadata: CFString

A key that indicates to generate per frame HDR Metadata and attach it to the resulting decoded pixel buffers.

let kVTDecompressionPropertyKey_DecoderProducesRAWOutput: CFString

let kVTDecompressionPropertyKey_RequestRAWOutput: CFString

### Multiview Decompression

let kVTDecompressionPropertyKey_RequestedMVHEVCVideoLayerIDs: CFString

Requests multi-image decoding of specific MV-HEVC video layers.

## See Also

### Configuring a Session

func VTVideoDecoderExtensionProperties(CMFormatDescription) throws -> [VTExtensionPropertiesKey : Any]


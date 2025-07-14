

- Video Toolbox
- VTCompressionSession
-  Compression Properties 

API Collection

# Compression Properties

Properties that you use to configure a compression session.

## Overview

Note

Video encoders may not support all compression property keys.

## Topics

### Buffers

let kVTCompressionPropertyKey_NumberOfPendingFrames: CFString

The number of pending frames in the compression session.

let kVTCompressionPropertyKey_PixelBufferPoolIsShared: CFString

A Boolean value indicating whether the common pixel buffer pool is shared between the video encoder and the session client.

let kVTCompressionPropertyKey_VideoEncoderPixelBufferAttributes: CFString

The video encoder’s pixel buffer attributes for the compression session.

### Frame Dependency

let kVTCompressionPropertyKey_AllowFrameReordering: CFString

A Boolean value that indicates whether frame reordering is enabled.

let kVTCompressionPropertyKey_AllowOpenGOP: CFString

Enables Open GOP (Group Of Pictures) encoding.

let kVTCompressionPropertyKey_AllowTemporalCompression: CFString

A Boolean value indicating whether temporal compression is enabled.

let kVTCompressionPropertyKey_MaxKeyFrameInterval: CFString

The maximum interval between key frames, also known as the key frame rate.

let kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration: CFString

The maximum duration from one key frame to the next in seconds.

### Rate Control

let kVTCompressionPropertyKey_AverageBitRate: CFString

The long-term desired average bit rate in bits per second.

let kVTCompressionPropertyKey_ConstantBitRate: CFString

Requires that the encoder use a Constant Bit Rate algorithm.

let kVTCompressionPropertyKey_DataRateLimits: CFString

Zero, one, or two hard limits on data rate.

let kVTCompressionPropertyKey_EstimatedAverageBytesPerFrame: CFString

An estimate of the expected size in bytes of a single encoded frame based on the current configuration.

let kVTCompressionPropertyKey_MoreFramesAfterEnd: CFString

A Boolean value indicating whether and how a compression session concatenates frames with other compressed frames to form a longer series.

let kVTCompressionPropertyKey_MoreFramesBeforeStart: CFString

A Boolean value that indicates whether and how a compression session concatenates frames with other compressed frames to form a longer series.

let kVTCompressionPropertyKey_Quality: CFString

The desired compression quality.

let kVTCompressionPropertyKey_TargetQualityForAlpha: CFString

The target quality to use for encoding the alpha channel.

### Bitstream Configuration

let kVTCompressionPropertyKey_PreserveAlphaChannel: CFString

A key that specifies whether to encode the alpha channel of input video frames.

let kVTCompressionPropertyKey_Depth: CFString

The pixel depth of the encoded video.

let kVTCompressionPropertyKey_H264EntropyMode: CFString

The entropy encoding mode for H.264 compression.

let kVTCompressionPropertyKey_HDRMetadataInsertionMode: CFString

let kVTCompressionPropertyKey_OutputBitDepth: CFString

let kVTCompressionPropertyKey_ProfileLevel: CFString

The profile and level for the encoded bitstream.

### Runtime Restrictions

let kVTCompressionPropertyKey_MaxFrameDelayCount: CFString

The maximum number of frames that a compressor is allowed to hold before it must output a compressed frame.

let kVTCompressionPropertyKey_MaxH264SliceBytes: CFString

The maximum slice size for H.264 encoding.

let kVTCompressionPropertyKey_MaximizePowerEfficiency: CFString

let kVTCompressionPropertyKey_RealTime: CFString

A Boolean value indicating whether it’s recommended that the video encoder perform compression in real time.

### Hints

let kVTCompressionPropertyKey_BaseLayerBitRateFraction: CFString

let kVTCompressionPropertyKey_BaseLayerFrameRate: CFString

let kVTCompressionPropertyKey_BaseLayerFrameRateFraction: CFString

let kVTCompressionPropertyKey_ExpectedDuration: CFString

The expected total duration of the compression session, if known.

let kVTCompressionPropertyKey_ExpectedFrameRate: CFString

The expected frame rate, if known.

let kVTCompressionPropertyKey_MaximumRealTimeFrameRate: CFString

A value that specifies the maximum real time rate at which frames can be submitted to a compression session.

let kVTCompressionPropertyKey_PrioritizeEncodingSpeedOverQuality: CFString

A hint for the video encoder to maximize its speed during encoding, sacrificing quality if needed.

let kVTCompressionPropertyKey_ReferenceBufferCount: CFString

let kVTCompressionPropertyKey_SourceFrameCount: CFString

The number of source frames, if known.

let kVTCompressionPropertyKey_CalculateMeanSquaredError: CFString

let kVTCompressionPropertyKey_HasLeftStereoEyeView: CFString

let kVTCompressionPropertyKey_HasRightStereoEyeView: CFString

let kVTCompressionPropertyKey_HorizontalFieldOfView: CFString

let kVTSampleAttachmentKey_QualityMetrics: CFString

let kVTSampleAttachmentQualityMetricsKey_ChromaBlueMeanSquaredError: CFString

let kVTSampleAttachmentQualityMetricsKey_ChromaRedMeanSquaredError: CFString

let kVTSampleAttachmentQualityMetricsKey_LumaMeanSquaredError: CFString

### Hardware Acceleration

let kVTCompressionPropertyKey_SupportsBaseFrameQP: CFString

A value that indicates whether the encoder supports base frame QP requests.

let kVTCompressionPropertyKey_UsingGPURegistryID: CFString

let kVTCompressionPropertyKey_UsingHardwareAcceleratedVideoEncoder: CFString

A Boolean value indicating whether a hardware-accelerated video encoder is used.

let kVTVideoEncoderSpecification_EnableHardwareAcceleratedVideoEncoder: CFString

A Boolean value indicating whether hardware-accelerated video encoding is allowed, if available.

let kVTVideoEncoderSpecification_PreferredEncoderGPURegistryID: CFString

let kVTVideoEncoderSpecification_RequireHardwareAcceleratedVideoEncoder: CFString

A Boolean value indicating whether hardware-accelerated encoding is required.

let kVTVideoEncoderSpecification_RequiredEncoderGPURegistryID: CFString

### Per-Frame Configuration

let kVTEncodeFrameOptionKey_BaseFrameQP: CFString

let kVTEncodeFrameOptionKey_ForceKeyFrame: CFString

Boolean value indicating whether the current frame is forced to be a key frame.

### Clean Aperture and Pixel Aspect Ratio

let kVTCompressionPropertyKey_AspectRatio16x9: CFString

A Boolean value indicating whether the DV video stream should have the 16x9 flag set.

let kVTCompressionPropertyKey_CleanAperture: CFString

The clean aperture for encoded frames.

let kVTCompressionPropertyKey_FieldCount: CFString

The field count indicating whether the frames should be encoded progressive (1) or interlaced (2).

let kVTCompressionPropertyKey_FieldDetail: CFString

Field ordering for encoded interlaced frames.

let kVTCompressionPropertyKey_PixelAspectRatio: CFString

The pixel aspect ratio for encoded frames.

let kVTCompressionPropertyKey_ProgressiveScan: CFString

A Boolean value indicating whether the DV video stream should have the progressive flag set.

### Color

let kVTCompressionPropertyKey_AlphaChannelMode: CFString

let kVTCompressionPropertyKey_ColorPrimaries: CFString

The color primaries for compressed content.

let kVTCompressionPropertyKey_ContentLightLevelInfo: CFString

let kVTCompressionPropertyKey_GammaLevel: CFString

let kVTCompressionPropertyKey_ICCProfile: CFString

The ICC profile for compressed content.

let kVTCompressionPropertyKey_MasteringDisplayColorVolume: CFString

let kVTCompressionPropertyKey_TransferFunction: CFString

The transfer function for compressed content.

let kVTCompressionPropertyKey_YCbCrMatrix: CFString

The YCbCr matrix for compressed content.

### Precompression Processing

let kVTCompressionPropertyKey_PixelTransferProperties: CFString

Properties for configuring a pixel transfer session.

### Multipass Storage

let kVTCompressionPropertyKey_MultiPassStorage: CFString

A property key that enables multipass compression and provides storage for encoder private data.

### Encoder Information

let kVTVideoEncoderSpecification_EncoderID: CFString

A key that indicates a particular video encoder to use.

let kVTCompressionPropertyKey_RecommendedParallelizationLimit: CFString

The recommended number of compression sessions to instantiate in a parallel encoding configuration.

let kVTCompressionPropertyKey_RecommendedParallelizedSubdivisionMinimumDuration: CFString

The recommended minimum duration for a given subdivision in a parallel encoding configuration.

let kVTCompressionPropertyKey_RecommendedParallelizedSubdivisionMinimumFrameCount: CFString

The recommended minimum number of video frames for a given subdivision in a parallel encoding configuration.

let kVTCompressionPropertyKey_EnableLTR: CFString

Enables Long Term Reference (LTR) frames during encoding.

let kVTCompressionPropertyKey_EncoderID: CFString

Specifies a particular video encoder by its ID string.

let kVTCompressionPropertyKey_MinAllowedFrameQP: CFString

The minimum allowed encoded frame QP (Quantization Parameter).

let kVTCompressionPropertyKey_MaxAllowedFrameQP: CFString

The maximum allowed encoded frame QP (Quantization Parameter).

let kVTCompressionPropertyKey_PreserveDynamicHDRMetadata: CFString

Specifies whether to preserve dynamic HDR metadata on the input pixel buffer.

let kVTEncodeFrameOptionKey_AcknowledgedLTRTokens: CFString

Enable Long Term Reference (LTR) frames during encoding.

let kVTEncodeFrameOptionKey_ForceLTRRefresh: CFString

A Boolean value that indicates whether to force Long Term Reference (LTR).

let kVTSampleAttachmentKey_RequireLTRAcknowledgementToken: CFString

A number value that contains a unique token for this Long Term Reference (LTR).

let kVTVideoEncoderSpecification_EnableLowLatencyRateControl: CFString

Specifies to select an encoder that supports low-latency operation and enables low-latency mode.

let kVTCompressionPropertyKey_SpatialAdaptiveQPLevel: CFString

A value that controls spatial adaptation of the quantization parameter (QP) based on per-frame statistics.

let kVTCompressionPropertyKey_SuggestedLookAheadFrameCount: CFString

A value that requests that the encoder retain the specified number of frames during encoding.

### Video Extended Usage (VEXU) Signaling

let kVTCompressionPropertyKey_HeroEye: CFString

A value that indicates which eye is the primary eye when rendering in 2D.

let kVTCompressionPropertyKey_StereoCameraBaseline: CFString

A value that specifies the distance between centers of the lenses of the camera system.

let kVTCompressionPropertyKey_HorizontalDisparityAdjustment: CFString

A value that indicates a relative shift of the left and right images, which changes the zero parallax plane.

let kVTCompressionPropertyKey_ProjectionKind: CFString

A value that indicates the projection kind.

let kVTCompressionPropertyKey_ViewPackingKind: CFString

A value that indicates the view packing kind.

### Multiview compression

let kVTCompressionPropertyKey_MVHEVCVideoLayerIDs: CFString

The identifiers of the video layers to encode in a multiview encoding operation.

let kVTCompressionPropertyKey_MVHEVCViewIDs: CFString

The identifiers of the views corresponding to the video layers in a multiview encoding operation.

let kVTCompressionPropertyKey_MVHEVCLeftAndRightViewIDs: CFString

Specifies which view identifier corresponds to the left eye and right eye.


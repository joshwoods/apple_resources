

- Core Media
-  kCMSampleBufferAttachmentKey_CameraIntrinsicMatrix 

Global Variable

# kCMSampleBufferAttachmentKey_CameraIntrinsicMatrix

An attachment that indicates a 3x3 camera intrinsic matrix to apply to the current sample buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleBufferAttachmentKey_CameraIntrinsicMatrix: CFString
```

## See Also

### Constants

var kCMAttachmentMode_ShouldNotPropagate: CMAttachmentMode

A mode that doesn’t propagate attachments to another object.

var kCMAttachmentMode_ShouldPropagate: CMAttachmentMode

A mode that propagates attachments to another object.

let kCMSampleAttachmentKey_HEVCTemporalLevelInfo: CFString

An attachment that indicates a video frame’s level within a hierarchical frame dependency structure.

let kCMSampleAttachmentKey_HEVCTemporalSubLayerAccess: CFString

An attachment that indicates a temporal sublayer access grouping.

let kCMSampleAttachmentKey_HEVCStepwiseTemporalSubLayerAccess: CFString

An attachment that indicates a step-wise temporal sublayer access (STSA) sample grouping.

let kCMSampleAttachmentKey_HEVCSyncSampleNALUnitType: CFString

An attachment that indicates a sync sample NAL unit type.

let kCMSampleAttachmentKey_CryptorSubsampleAuxiliaryData: CFString

An attachment that describes the ranges of protected and unprotected data within a protected sample buffer.

let kCMSampleAttachmentKey_AudioIndependentSampleDecoderRefreshCount: CFString

An attachment that’s only present if the audio sample is an independent frame or immediate playout frame.


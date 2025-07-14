

- Core Media
-  kCMSampleAttachmentKey_CryptorSubsampleAuxiliaryData 

Global Variable

# kCMSampleAttachmentKey_CryptorSubsampleAuxiliaryData

An attachment that describes the ranges of protected and unprotected data within a protected sample buffer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let kCMSampleAttachmentKey_CryptorSubsampleAuxiliaryData: CFString
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

let kCMSampleAttachmentKey_AudioIndependentSampleDecoderRefreshCount: CFString

An attachment that’s only present if the audio sample is an independent frame or immediate playout frame.

let kCMSampleBufferAttachmentKey_CameraIntrinsicMatrix: CFString

An attachment that indicates a 3x3 camera intrinsic matrix to apply to the current sample buffer.


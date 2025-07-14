

- Core Media
-  CMAttachment APIs 

API Collection

# CMAttachment APIs

Add supporting metadata to sample buffers.

## Overview

An attachment bearer is a Core Foundation type object that supports the suite of key, value, and mode attachment APIs. You can attach any Core Foundation object to an attachment bearer to store additional information.

## Topics

### Processing Attachments

func CMGetAttachment(CMAttachmentBearer, key: CFString, attachmentModeOut: UnsafeMutablePointer&lt;CMAttachmentMode>?) -> CFTypeRef?

Returns an attachment from an attachment bearer object.

func CMCopyDictionaryOfAttachments(allocator: CFAllocator?, target: CMAttachmentBearer, attachmentMode: CMAttachmentMode) -> CFDictionary?

Returns a dictionary of all attachments for an attachment bearer object.

func CMSetAttachment(CMAttachmentBearer, key: CFString, value: CFTypeRef?, attachmentMode: CMAttachmentMode)

Sets or adds an attachment to an attachment bearer object.

func CMSetAttachments(CMAttachmentBearer, attachments: CFDictionary, attachmentMode: CMAttachmentMode)

Sets a dictionary of attachments on an attachment bearer object.

func CMRemoveAttachment(CMAttachmentBearer, key: CFString)

Removes a specific attachment from an attachment bearer object.

func CMRemoveAllAttachments(CMAttachmentBearer)

Removes all attachments from an attachment bearer object.

func CMPropagateAttachments(CMAttachmentBearer, destination: CMAttachmentBearer)

Copies all propagable attachments from one attachment bearer object to another.

### Data Types

protocol CMAttachmentBearerProtocol

A protocol for objects that can carry attachments.

typealias CMAttachmentBearer

An object that can carry attachments.

typealias CMAttachmentMode

The mode to use when propagating attachments.

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

let kCMSampleBufferAttachmentKey_CameraIntrinsicMatrix: CFString

An attachment that indicates a 3x3 camera intrinsic matrix to apply to the current sample buffer.

## See Also

### Sample Processing

CMSampleBuffer APIs

An object that contains zero or more media samples of a uniform media type.

CMBlockBuffer APIs

An object the system uses to move blocks of memory through a processing system.

struct CMTaggedBuffer

An instance of a media buffer containing metadata tags.

CMTaggedBufferGroup APIs

Objective-C types and interfaces for working with Core Media tagged buffer groups.

CMFormatDescription APIs

A media format descriptor that describes the samples in a sample buffer.


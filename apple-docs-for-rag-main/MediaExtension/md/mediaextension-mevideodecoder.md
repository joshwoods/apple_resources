

- MediaExtension
-  MEVideoDecoder 

Protocol

# MEVideoDecoder

A protocol that defines the requirements for a video decoder.

macOS 14.0+

``` source
protocol MEVideoDecoder : NSObjectProtocol
```

## Overview

This protocol provides an interface for Video Toolbox to create and interact with MediaExtension video decoders. `MEVideoDecoder` objects are always instantiated by Video Toolbox.

Note

Developers who wish to build MediaExtension video decoders using this API need to include a Video decoder entitlement, provisioning profile, and specialized dictionary in their Info.plist file when building their extensions.

For more information, see Entitlements, Create a development provisioning profile, and Video decoder property list dictionary

Once a user installs and runs the host app, embedded video decoder extensions become available to any app on the user’s system that opts in to using them by calling VTRegisterProfessionalVideoWorkflowVideoDecoders().

Important

`MEVideoDecoder` objects run in a sandboxed process without access to the filesystem, network, and other kernel resources.

The following sections explain the video decoder life cycle and performing decoding operations.

### Creating a video decoder

The first time Video Toolbox opens a decoder in a process, it creates an instance of the MEVideoDecoderExtension factory object. It then calls its makeVideoDecoder(codecType:videoFormatDescription:videoDecoderSpecifications:pixelBufferManager:) method for each decoder instance it needs. A decoder can evaluate the CMVideoCodecType and CMVideoFormatDescription that the system provides and confirm whether it can decode the specified format. If the decoder can’t decode the format, the factory routine needs to return the error MEError.Code.unsupportedFeature. This sequence of events happens within VTDecompressionSessionCreate(allocator:formatDescription:decoderSpecification:imageBufferAttributes:outputCallback:decompressionSessionOut:).

### Configuring a pixel buffer

Once instantiated, a decoder can call back to the provided MEVideoDecoderPixelBufferManager object to notify Video Toolbox of its output CVPixelBuffer requirements. It can make these calls multiple times if output requirements change in response to properties receiving new values or due to observed bitstream characteristics.

### Querying and setting properties

Properties can receive queries or new values on the decoder at any time, before, during or after frame decode, unless otherwise noted. These calls generally correspond to VTSessionSetProperty(_:key:value:) and VTSessionCopyProperty(_:key:allocator:valueOut:) calls on the VTDecompressionSession which opened the decoder. There may be cases where Video Toolbox directly sets or queries properties as well.

### Decoding frames

The framework serializes calls to decodeFrame(from:options:completionHandler:) and doesn’t send a new frame to the decoder until the last decodeFrame(from:options:completionHandler:) returns, unless decoding happens asynchronously. These calls correspond to VTDecompressionSessionDecodeFrame(_:sampleBuffer:flags:infoFlagsOut:outputHandler:) calls on the owning `VTDecompressionSession`.

Video decoders need to write their output frames into CVPixelBuffer objects allocated by the MEVideoDecoderPixelBufferManager object’s makePixelBuffer() method. Obtaining pixel buffers from any other source may degrade performance or result in other issues.

If the decoder’s internal decoding queue is full and it can’t decode more frames, its isReadyForMoreMediaData property value returns false. It returns true once the decoder can start accepting new frames again. This generally occurs after an earlier asynchronous frame completes.

### Handling format description changes

If a change occurs in the format description on incoming CMSampleBuffer objects, Video Toolbox calls canAccept(_:) to confirm whether the decoder can transition to the new format description. If that method response is false, the system usually closes the decoder and creates a new instance for the changed format description. A call to VTDecompressionSessionCanAcceptFormatDescription(_:formatDescription:) can trigger a call of canAccept(_:), or Video Toolbox calls this method if it sees a format description change on incoming `CMSampleBufferRef` objects.

## Topics

### Inspecting a video decoder

var contentHasInterframeDependencies: Bool

A Boolean that specifies whether the content has interframe dependencies, if the decoder knows.

var recommendedThreadCount: Int

The recommended number of threads for the decoder to use.

var actualThreadCount: Int

The actual number of threads the decoder uses.

var supportedPixelFormatsOrderedByQuality: [NSNumber]

Provides hints about quality tradeoffs between pixel formats.

var reducedResolution: CGSize

A request to decode at a lower resolution than full-size.

var pixelFormatsWithReducedResolutionDecodeSupport: [NSNumber]

Provides a list of output pixel formats where the decoder supports reduced resolution decoding.

var producesRAWOutput: Bool

Indicates whether the decoder produces RAW output which requires the use of a RAW processor.

var isReadyForMoreMediaData: Bool

A Boolean value that indicates the readiness of the decoder to accept more sample buffers.

**Required**

### Decoding frames

func canAccept(CMFormatDescription) -> Bool

Asks the extension whether the decoder can decode frames with the format description that you specify.

func decodeFrame(from: CMSampleBuffer, options: MEDecodeFrameOptions, completionHandler: (CVImageBuffer?, MEDecodeFrameStatus, (any Error)?) -> Void)

Requests the extension to decode a video frame.

**Required**

struct MEDecodeFrameStatus

A type that represents a non-error status related to a frame decode operation.

### Extension requirements

Video decoder property list dictionary

Include a property list dictionary to describe a video decoder.

Video decoder entitlement

Include an entitlement to indicate your extension is a MediaExtension video decoder.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Video decoders

protocol MEVideoDecoderExtension

A protocol that defines a factory to create new video decoders for a codec type that the extension implements.

class MEDecodeFrameOptions

An object that guides the video decoder operation on a per-frame basis.

class MEVideoDecoderPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

Video decoder property list dictionary

Include a property list dictionary to describe a video decoder.

Video decoder entitlement

Include an entitlement to indicate your extension is a MediaExtension video decoder.


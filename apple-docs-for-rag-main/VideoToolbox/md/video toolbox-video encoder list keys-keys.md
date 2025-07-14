

- Video Toolbox
-  Video Encoder List Keys 

API Collection

# Video Encoder List Keys

Dictionary key constants to use to retrieve video encoder information.

## Overview

Use these keys to pass to the VTCopyVideoEncoderList(_:_:) function.

## Topics

### Encoder Keys

let kVTVideoEncoderList_EncoderID: CFString

A key that identifies the encoder ID.

let kVTVideoEncoderList_EncoderName: CFString

A key for the encoder’s name.

let kVTVideoEncoderList_DisplayName: CFString

The encoder’s display name key.

let kVTVideoEncoderList_CodecType: CFString

The encoder’s codec type key.

let kVTVideoEncoderList_CodecName: CFString

The encoder’s codec name key.

let kVTVideoEncoderList_GPURegistryID: CFString

let kVTVideoEncoderList_InstanceLimit: CFString

let kVTVideoEncoderList_IsHardwareAccelerated: CFString

let kVTVideoEncoderList_PerformanceRating: CFString

let kVTVideoEncoderList_QualityRating: CFString

let kVTVideoEncoderList_SupportedSelectionProperties: CFString

let kVTVideoEncoderList_SupportsFrameReordering: CFString

let kVTVideoEncoderListOption_IncludeStandardDefinitionDVEncoders: CFString

## See Also

### Codec Support

func VTIsHardwareDecodeSupported(CMVideoCodecType) -> Bool

Returns a Boolean value that indicates whether the current system supports hardware decode for the specified codec.

func VTRegisterProfessionalVideoWorkflowVideoEncoders()

Loads encoders appropriate for the client’s professional video workflows.

func VTRegisterProfessionalVideoWorkflowVideoDecoders()

Loads decoders appropriate for the client’s professional video workflows.

func VTRegisterSupplementalVideoDecoderIfAvailable(CMVideoCodecType)

Registers a video decoder for the specified codec type, if one exists on the current system.

func VTCopySupportedPropertyDictionaryForEncoder(width: Int32, height: Int32, codecType: CMVideoCodecType, encoderSpecification: CFDictionary?, encoderIDOut: UnsafeMutablePointer&lt;CFString?>?, supportedPropertiesOut: UnsafeMutablePointer&lt;CFDictionary?>?) -> OSStatus

Builds a list of supported properties and encoder ID for an encoder.

func VTCopyVideoEncoderList(CFDictionary?, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Builds a list of available video encoders.


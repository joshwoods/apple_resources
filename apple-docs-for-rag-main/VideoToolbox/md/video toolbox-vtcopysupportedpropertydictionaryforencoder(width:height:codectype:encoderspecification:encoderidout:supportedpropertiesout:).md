

- Video Toolbox
-  VTCopySupportedPropertyDictionaryForEncoder(width:height:codecType:encoderSpecification:encoderIDOut:supportedPropertiesOut:) 

Function

# VTCopySupportedPropertyDictionaryForEncoder(width:height:codecType:encoderSpecification:encoderIDOut:supportedPropertiesOut:)

Builds a list of supported properties and encoder ID for an encoder.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func VTCopySupportedPropertyDictionaryForEncoder(
    width: Int32,
    height: Int32,
    codecType: CMVideoCodecType,
    encoderSpecification: CFDictionary?,
    encoderIDOut: UnsafeMutablePointer?,
    supportedPropertiesOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`width`  

`height`  

`codecType`  

`encoderSpecification`  

`encoderIDOut`  

`supportedPropertiesOut`  

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

func VTCopyVideoEncoderList(CFDictionary?, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Builds a list of available video encoders.

Video Encoder List Keys

Dictionary key constants to use to retrieve video encoder information.


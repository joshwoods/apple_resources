

- Video Toolbox
-  VTRegisterSupplementalVideoDecoderIfAvailable(\_:) 

Function

# VTRegisterSupplementalVideoDecoderIfAvailable(\_:)

Registers a video decoder for the specified codec type, if one exists on the current system.

macOS 11.0+

``` source
func VTRegisterSupplementalVideoDecoderIfAvailable(_ codecType: CMVideoCodecType)
```

## Parameters 

`codecType`  

A codec type for which to register a decoder.

## Discussion

Call this function to find and register video decoders that aren’t registered by default.

## See Also

### Codec Support

func VTIsHardwareDecodeSupported(CMVideoCodecType) -> Bool

Returns a Boolean value that indicates whether the current system supports hardware decode for the specified codec.

func VTRegisterProfessionalVideoWorkflowVideoEncoders()

Loads encoders appropriate for the client’s professional video workflows.

func VTRegisterProfessionalVideoWorkflowVideoDecoders()

Loads decoders appropriate for the client’s professional video workflows.

func VTCopySupportedPropertyDictionaryForEncoder(width: Int32, height: Int32, codecType: CMVideoCodecType, encoderSpecification: CFDictionary?, encoderIDOut: UnsafeMutablePointer&lt;CFString?>?, supportedPropertiesOut: UnsafeMutablePointer&lt;CFDictionary?>?) -> OSStatus

Builds a list of supported properties and encoder ID for an encoder.

func VTCopyVideoEncoderList(CFDictionary?, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Builds a list of available video encoders.

Video Encoder List Keys

Dictionary key constants to use to retrieve video encoder information.




- Video Toolbox
-  VTIsHardwareDecodeSupported(\_:) 

Function

# VTIsHardwareDecodeSupported(\_:)

Returns a Boolean value that indicates whether the current system supports hardware decode for the specified codec.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func VTIsHardwareDecodeSupported(_ codecType: CMVideoCodecType) -> Bool
```

## Parameters 

`codecType`  

The codec for which to test for hardware decode support.

## Return Value

true if the current system supports hardware decode; otherwise, false.

## See Also

### Codec Support

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

Video Encoder List Keys

Dictionary key constants to use to retrieve video encoder information.


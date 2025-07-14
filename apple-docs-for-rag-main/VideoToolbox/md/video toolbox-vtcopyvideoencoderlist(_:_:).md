

- Video Toolbox
-  VTCopyVideoEncoderList(\_:\_:) 

Function

# VTCopyVideoEncoderList(\_:\_:)

Builds a list of available video encoders.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTCopyVideoEncoderList(
    _ options: CFDictionary?,
    _ listOfVideoEncodersOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`options`  

Not currently supported. Pass `NULL` for this parameter.

`listOfVideoEncodersOut`  

Pointer to a `CFArray` of available video encoders.

## Discussion

The caller must release the returned list using CFRelease.

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

Video Encoder List Keys

Dictionary key constants to use to retrieve video encoder information.


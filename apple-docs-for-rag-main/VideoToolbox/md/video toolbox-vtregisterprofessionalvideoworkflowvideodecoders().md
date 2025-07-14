

- Video Toolbox
-  VTRegisterProfessionalVideoWorkflowVideoDecoders() 

Function

# VTRegisterProfessionalVideoWorkflowVideoDecoders()

Loads decoders appropriate for the client’s professional video workflows.

macOS 10.9+

``` source
func VTRegisterProfessionalVideoWorkflowVideoDecoders()
```

## Discussion

This function loads the video decoders within the client’s `/Library/Video/Professional Video Workflow Plug-Ins/` directory, if any are present. Additionally, calling this function indicates to Video Toolbox that your app supports MediaExtension video decoders. Any associated video RAW Processors will also be supported as well.

Note

This functionality is only intended for apps that support professional video workflows. It isn’t recommended for network-facing applications such as web browsers, messaging clients, mail clients, and so on.

### Apple Afterburner Acceleration

Apple Afterburner is an accelerator card for the Mac Pro (2019), created to enhance Apple ProRes and ProRes RAW workflows for film and video professionals. Afterburner accelerates decoding and playback of multiple streams of ProRes and Pro Res RAW video files.

You must call this function to load the ProRes and ProRes RAW decoders so the Afterburner card can accelerate ProRes and ProRes RAW decoding and playback.

If the decoders aren’t loaded, the system performs nonaccelerated software playback and decoding of ProRes and ProRes RAW video files.

## See Also

### Codec Support

func VTIsHardwareDecodeSupported(CMVideoCodecType) -> Bool

Returns a Boolean value that indicates whether the current system supports hardware decode for the specified codec.

func VTRegisterProfessionalVideoWorkflowVideoEncoders()

Loads encoders appropriate for the client’s professional video workflows.

func VTRegisterSupplementalVideoDecoderIfAvailable(CMVideoCodecType)

Registers a video decoder for the specified codec type, if one exists on the current system.

func VTCopySupportedPropertyDictionaryForEncoder(width: Int32, height: Int32, codecType: CMVideoCodecType, encoderSpecification: CFDictionary?, encoderIDOut: UnsafeMutablePointer&lt;CFString?>?, supportedPropertiesOut: UnsafeMutablePointer&lt;CFDictionary?>?) -> OSStatus

Builds a list of supported properties and encoder ID for an encoder.

func VTCopyVideoEncoderList(CFDictionary?, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Builds a list of available video encoders.

Video Encoder List Keys

Dictionary key constants to use to retrieve video encoder information.


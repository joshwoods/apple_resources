

- Video Toolbox
-  kVTVideoEncoderList_DisplayName 

Global Variable

# kVTVideoEncoderList_DisplayName

The encoder’s display name key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTVideoEncoderList_DisplayName: CFString
```

## Discussion

The associated value is a doc://com.apple.documentation/documentation/corefoundation/cfstring-rfh with the encoder’s display name.

This value will be the same as the value of kVTVideoEncoderList_CodecName if there is only one encoder for that format; otherwise, it will be the same as the value of kVTVideoEncoderList_EncoderName.

## See Also

### Encoder Keys

let kVTVideoEncoderList_EncoderID: CFString

A key that identifies the encoder ID.

let kVTVideoEncoderList_EncoderName: CFString

A key for the encoder’s name.

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


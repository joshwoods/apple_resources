

- Video Toolbox
-  kVTVideoEncoderSpecification_EnableHardwareAcceleratedVideoEncoder 

Global Variable

# kVTVideoEncoderSpecification_EnableHardwareAcceleratedVideoEncoder

A Boolean value indicating whether hardware-accelerated video encoding is allowed, if available.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 10.9+tvOS 17.4+visionOS 1.1+

``` source
let kVTVideoEncoderSpecification_EnableHardwareAcceleratedVideoEncoder: CFString
```

## Discussion

This key is set in the `encoderSpecification` passed in to VTCompressionSessionCreate(allocator:width:height:codecType:encoderSpecification:imageBufferAttributes:compressedDataAllocator:outputCallback:refcon:compressionSessionOut:). Set it to kCFBooleanTrue to allow hardware-accelerated encoding. To specifically prevent hardware encoding, set this property to kCFBooleanFalse.

This setting is useful for clients doing realtime encoding operations because it allows VideoToolbox to choose the optimal encoding path.

## See Also

### Hardware Acceleration

let kVTCompressionPropertyKey_SupportsBaseFrameQP: CFString

A value that indicates whether the encoder supports base frame QP requests.

let kVTCompressionPropertyKey_UsingGPURegistryID: CFString

let kVTCompressionPropertyKey_UsingHardwareAcceleratedVideoEncoder: CFString

A Boolean value indicating whether a hardware-accelerated video encoder is used.

let kVTVideoEncoderSpecification_PreferredEncoderGPURegistryID: CFString

let kVTVideoEncoderSpecification_RequireHardwareAcceleratedVideoEncoder: CFString

A Boolean value indicating whether hardware-accelerated encoding is required.

let kVTVideoEncoderSpecification_RequiredEncoderGPURegistryID: CFString


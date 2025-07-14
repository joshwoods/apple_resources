

- Video Toolbox
-  kVTCompressionPropertyKey_UsingHardwareAcceleratedVideoEncoder 

Global Variable

# kVTCompressionPropertyKey_UsingHardwareAcceleratedVideoEncoder

A Boolean value indicating whether a hardware-accelerated video encoder is used.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 10.9+tvOS 17.4+visionOS 1.1+

``` source
let kVTCompressionPropertyKey_UsingHardwareAcceleratedVideoEncoder: CFString
```

## Discussion

You can query this property using VTSessionCopyProperty(_:key:allocator:valueOut:) after you have enabled hardware accelerated encode using kVTVideoEncoderSpecification_EnableHardwareAcceleratedVideoEncoder to see if a hardware-accelerated encoder was selected (kCFBooleanTrue).

## See Also

### Hardware Acceleration

let kVTCompressionPropertyKey_SupportsBaseFrameQP: CFString

A value that indicates whether the encoder supports base frame QP requests.

let kVTCompressionPropertyKey_UsingGPURegistryID: CFString

let kVTVideoEncoderSpecification_EnableHardwareAcceleratedVideoEncoder: CFString

A Boolean value indicating whether hardware-accelerated video encoding is allowed, if available.

let kVTVideoEncoderSpecification_PreferredEncoderGPURegistryID: CFString

let kVTVideoEncoderSpecification_RequireHardwareAcceleratedVideoEncoder: CFString

A Boolean value indicating whether hardware-accelerated encoding is required.

let kVTVideoEncoderSpecification_RequiredEncoderGPURegistryID: CFString


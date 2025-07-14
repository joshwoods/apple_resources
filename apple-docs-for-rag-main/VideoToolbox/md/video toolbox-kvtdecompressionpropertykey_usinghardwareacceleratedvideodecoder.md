

- Video Toolbox
-  kVTDecompressionPropertyKey_UsingHardwareAcceleratedVideoDecoder 

Global Variable

# kVTDecompressionPropertyKey_UsingHardwareAcceleratedVideoDecoder

Indicates if a hardware-accelerated video decoder is being used.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_UsingHardwareAcceleratedVideoDecoder: CFString
```

## Discussion

You can query this property using VTSessionCopyProperty(_:key:allocator:valueOut:) after you have enabled hardware accelerated decode using kVTVideoDecoderSpecification_EnableHardwareAcceleratedVideoDecoder to see if a hardware accelerated decoder was selected.

## See Also

### Hardware Acceleration

let kVTVideoDecoderSpecification_EnableHardwareAcceleratedVideoDecoder: CFString

A Boolean value indicating whether VideoToolbox uses a hardware-accelerated video decoder, if available.

let kVTVideoDecoderSpecification_RequireHardwareAcceleratedVideoDecoder: CFString

A Boolean value indicating whether to require hardware-accelerated decoding.


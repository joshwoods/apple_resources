

- Video Toolbox
-  kVTVideoDecoderSpecification_EnableHardwareAcceleratedVideoDecoder 

Global Variable

# kVTVideoDecoderSpecification_EnableHardwareAcceleratedVideoDecoder

A Boolean value indicating whether VideoToolbox uses a hardware-accelerated video decoder, if available.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
let kVTVideoDecoderSpecification_EnableHardwareAcceleratedVideoDecoder: CFString
```

## Discussion

You set this key in the `decoderSpecification` passed in to VTDecompressionSessionCreate(allocator:formatDescription:decoderSpecification:imageBufferAttributes:outputCallback:decompressionSessionOut:). Set it to kCFBooleanTrue to allow hardware-accelerated decoding. To specifically prevent hardware-accelerated decoding, set this property to kCFBooleanFalse. This property is useful for clients doing realtime decode operations because it allows VideoToolbox to choose the optimal decoding path.

## See Also

### Hardware Acceleration

let kVTVideoDecoderSpecification_RequireHardwareAcceleratedVideoDecoder: CFString

A Boolean value indicating whether to require hardware-accelerated decoding.

let kVTDecompressionPropertyKey_UsingHardwareAcceleratedVideoDecoder: CFString

Indicates if a hardware-accelerated video decoder is being used.


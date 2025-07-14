

- Video Toolbox
-  kVTCompressionPropertyKey_MaxH264SliceBytes 

Global Variable

# kVTCompressionPropertyKey_MaxH264SliceBytes

The maximum slice size for H.264 encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_MaxH264SliceBytes: CFString
```

## Discussion

If supported by an H.264 encoder, the value limits the size in bytes of slices produced by the encoder, where possible. By default, no limit is specified. A value of zero implies default behavior.

## See Also

### Runtime Restrictions

let kVTCompressionPropertyKey_MaxFrameDelayCount: CFString

The maximum number of frames that a compressor is allowed to hold before it must output a compressed frame.

let kVTCompressionPropertyKey_MaximizePowerEfficiency: CFString

let kVTCompressionPropertyKey_RealTime: CFString

A Boolean value indicating whether it’s recommended that the video encoder perform compression in real time.


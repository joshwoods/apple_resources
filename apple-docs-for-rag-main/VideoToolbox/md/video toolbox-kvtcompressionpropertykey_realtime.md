

- Video Toolbox
-  kVTCompressionPropertyKey_RealTime 

Global Variable

# kVTCompressionPropertyKey_RealTime

A Boolean value indicating whether it’s recommended that the video encoder perform compression in real time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_RealTime: CFString
```

## Discussion

For offline compression, clients may set this property to kCFBooleanFalse, which indicates that it is OK for the video encoder to work slower than real time in order to produce a better result.

For real-time compression, clients may set this property to kCFBooleanTrue to recommend that encoding stay timely.

By default, this property is `NULL`, indicating unknown.

## See Also

### Runtime Restrictions

let kVTCompressionPropertyKey_MaxFrameDelayCount: CFString

The maximum number of frames that a compressor is allowed to hold before it must output a compressed frame.

let kVTCompressionPropertyKey_MaxH264SliceBytes: CFString

The maximum slice size for H.264 encoding.

let kVTCompressionPropertyKey_MaximizePowerEfficiency: CFString


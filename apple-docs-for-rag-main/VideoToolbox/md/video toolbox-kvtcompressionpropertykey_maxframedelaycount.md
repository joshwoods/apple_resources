

- Video Toolbox
-  kVTCompressionPropertyKey_MaxFrameDelayCount 

Global Variable

# kVTCompressionPropertyKey_MaxFrameDelayCount

The maximum number of frames that a compressor is allowed to hold before it must output a compressed frame.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_MaxFrameDelayCount: CFString
```

## Discussion

This value limits the number of frames that may be held in the compression window. If the maximum frame delay count is M, then before the call to encode frame N returns, frame N-M must have been emitted. The default is kVTUnlimitedFrameDelayCount, which sets no limit on the compression window.

## Topics

### Delay Counts

var kVTUnlimitedFrameDelayCount: Int

Indicates that no limit should be set on the compression window.

## See Also

### Runtime Restrictions

let kVTCompressionPropertyKey_MaxH264SliceBytes: CFString

The maximum slice size for H.264 encoding.

let kVTCompressionPropertyKey_MaximizePowerEfficiency: CFString

let kVTCompressionPropertyKey_RealTime: CFString

A Boolean value indicating whether it’s recommended that the video encoder perform compression in real time.


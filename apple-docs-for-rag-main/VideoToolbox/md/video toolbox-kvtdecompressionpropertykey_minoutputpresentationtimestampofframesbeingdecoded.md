

- Video Toolbox
-  kVTDecompressionPropertyKey_MinOutputPresentationTimeStampOfFramesBeingDecoded 

Global Variable

# kVTDecompressionPropertyKey_MinOutputPresentationTimeStampOfFramesBeingDecoded

The minimum output presentation timestamp of the frames currently being decoded.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_MinOutputPresentationTimeStampOfFramesBeingDecoded: CFString
```

## Discussion

This value may change asynchronously as frames are output.

## See Also

### Asynchronous State

let kVTDecompressionPropertyKey_NumberOfFramesBeingDecoded: CFString

Returns the number of frames currently being decoded.

let kVTDecompressionPropertyKey_MaxOutputPresentationTimeStampOfFramesBeingDecoded: CFString

The maximum output presentation timestamp of the frames currently being decoded.


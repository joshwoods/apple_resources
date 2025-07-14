

- Video Toolbox
-  kVTDecompressionPropertyKey_NumberOfFramesBeingDecoded 

Global Variable

# kVTDecompressionPropertyKey_NumberOfFramesBeingDecoded

Returns the number of frames currently being decoded.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_NumberOfFramesBeingDecoded: CFString
```

## Discussion

This number may decrease asynchronously as frames are output.

## See Also

### Asynchronous State

let kVTDecompressionPropertyKey_MinOutputPresentationTimeStampOfFramesBeingDecoded: CFString

The minimum output presentation timestamp of the frames currently being decoded.

let kVTDecompressionPropertyKey_MaxOutputPresentationTimeStampOfFramesBeingDecoded: CFString

The maximum output presentation timestamp of the frames currently being decoded.




- Image I/O
-  kCGImagePropertyWebPFrameInfoArray 

Global Variable

# kCGImagePropertyWebPFrameInfoArray

An array of dictionaries that contain timing information for the image sequence.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGImagePropertyWebPFrameInfoArray: CFString
```

## Discussion

The value of this property is a CFArray. Each CFDictionary in the array contains timing information about an image in the sequence.

## See Also

### Sequence Timing

let kCGImagePropertyWebPDelayTime: CFString

The number of seconds to wait before displaying the next image in the sequence.

let kCGImagePropertyWebPUnclampedDelayTime: CFString

The unadjusted number of seconds to wait before displaying the next image in the sequence.

let kCGImagePropertyWebPLoopCount: CFString

The number of times to play the sequence.


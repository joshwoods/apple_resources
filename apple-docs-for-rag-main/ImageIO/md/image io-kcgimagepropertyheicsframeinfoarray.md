

- Image I/O
-  kCGImagePropertyHEICSFrameInfoArray 

Global Variable

# kCGImagePropertyHEICSFrameInfoArray

An array of dictionaries that contain timing information for the image sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let kCGImagePropertyHEICSFrameInfoArray: CFString
```

## Discussion

The value of this property is a CFArray. Each CFDictionary in the array contains timing information about an image in the sequence.

## See Also

### Sequence Timing

let kCGImagePropertyHEICSDelayTime: CFString

The number of seconds to wait before displaying the next image in the sequence, clamped to a minimum of `0.1` seconds.

let kCGImagePropertyHEICSUnclampedDelayTime: CFString

The unclamped number of seconds to wait before displaying the next image in the sequence.

let kCGImagePropertyHEICSLoopCount: CFString

The number of times to play the sequence.




- Image I/O
-  kCGImagePropertyGIFFrameInfoArray 

Global Variable

# kCGImagePropertyGIFFrameInfoArray

An array of dictionaries that contain timing information for the image sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let kCGImagePropertyGIFFrameInfoArray: CFString
```

## Discussion

The value of this property is a CFArray. Each CFDictionary in the array contains timing information about an image in the sequence.

## See Also

### Sequence Timing

let kCGImagePropertyGIFDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence, clamped to a minimum of 100 milliseconds.

let kCGImagePropertyGIFUnclampedDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyGIFLoopCount: CFString

The number of times to repeat an animated sequence.


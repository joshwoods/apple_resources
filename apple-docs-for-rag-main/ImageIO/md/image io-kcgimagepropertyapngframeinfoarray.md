

- Image I/O
-  kCGImagePropertyAPNGFrameInfoArray 

Global Variable

# kCGImagePropertyAPNGFrameInfoArray

An array of dictionaries that contain timing information for the image sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let kCGImagePropertyAPNGFrameInfoArray: CFString
```

## Discussion

The value of this property is a CFArray. Each CFDictionary in the array contains timing information about an image in the sequence.

## See Also

### Sequence Timing

let kCGImagePropertyAPNGDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyAPNGUnclampedDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyAPNGLoopCount: CFString

The number of times that an animated PNG should play through its frames before stopping.


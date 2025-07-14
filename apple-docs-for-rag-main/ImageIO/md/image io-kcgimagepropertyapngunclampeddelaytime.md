

- Image I/O
-  kCGImagePropertyAPNGUnclampedDelayTime 

Global Variable

# kCGImagePropertyAPNGUnclampedDelayTime

The number of seconds to wait before displaying the next image in an animated sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyAPNGUnclampedDelayTime: CFString
```

## Discussion

This value may be `0` milliseconds or higher. Unlike the kCGImagePropertyAPNGDelayTime property, this value is not clamped at the low end of the range.

## See Also

### Sequence Timing

let kCGImagePropertyAPNGFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyAPNGDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyAPNGLoopCount: CFString

The number of times that an animated PNG should play through its frames before stopping.


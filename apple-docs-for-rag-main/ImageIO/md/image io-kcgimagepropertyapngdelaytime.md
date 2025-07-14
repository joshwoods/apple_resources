

- Image I/O
-  kCGImagePropertyAPNGDelayTime 

Global Variable

# kCGImagePropertyAPNGDelayTime

The number of seconds to wait before displaying the next image in an animated sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyAPNGDelayTime: CFString
```

## Discussion

The value of this key is a CFNumber with a floating-point value. The value of this key is never less than 50 millseconds, and the system adjusts values less than that amount to 50 milliseconds, as needed. See kCGImagePropertyAPNGUnclampedDelayTime.

## See Also

### Sequence Timing

let kCGImagePropertyAPNGFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyAPNGUnclampedDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyAPNGLoopCount: CFString

The number of times that an animated PNG should play through its frames before stopping.


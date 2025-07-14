

- Image I/O
-  kCGImagePropertyGIFUnclampedDelayTime 

Global Variable

# kCGImagePropertyGIFUnclampedDelayTime

The number of seconds to wait before displaying the next image in an animated sequence.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyGIFUnclampedDelayTime: CFString
```

## Discussion

This value may be `0` milliseconds or higher. Unlike the kCGImagePropertyGIFDelayTime property, this value is not clamped at the low end of the range.

## See Also

### Sequence Timing

let kCGImagePropertyGIFFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyGIFDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence, clamped to a minimum of 100 milliseconds.

let kCGImagePropertyGIFLoopCount: CFString

The number of times to repeat an animated sequence.


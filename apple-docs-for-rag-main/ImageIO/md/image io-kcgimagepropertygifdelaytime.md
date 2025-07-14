

- Image I/O
-  kCGImagePropertyGIFDelayTime 

Global Variable

# kCGImagePropertyGIFDelayTime

The number of seconds to wait before displaying the next image in an animated sequence, clamped to a minimum of 100 milliseconds.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyGIFDelayTime: CFString
```

## Discussion

The value of this key is a CFNumber with a floating-point value. The value of this key is never less than 100 millseconds, and the system adjusts values less than that amount to 100 milliseconds, as needed. See kCGImagePropertyGIFUnclampedDelayTime.

## See Also

### Sequence Timing

let kCGImagePropertyGIFFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyGIFUnclampedDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyGIFLoopCount: CFString

The number of times to repeat an animated sequence.


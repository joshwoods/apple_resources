

- Image I/O
-  kCGImagePropertyAPNGLoopCount 

Global Variable

# kCGImagePropertyAPNGLoopCount

The number of times that an animated PNG should play through its frames before stopping.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyAPNGLoopCount: CFString
```

## Discussion

A value of `0` means the PNG repeats forever.

## See Also

### Sequence Timing

let kCGImagePropertyAPNGFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyAPNGDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyAPNGUnclampedDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.


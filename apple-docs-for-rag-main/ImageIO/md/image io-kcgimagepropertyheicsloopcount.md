

- Image I/O
-  kCGImagePropertyHEICSLoopCount 

Global Variable

# kCGImagePropertyHEICSLoopCount

The number of times to play the sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let kCGImagePropertyHEICSLoopCount: CFString
```

## Discussion

The value of this key is a CFNumber.

## See Also

### Sequence Timing

let kCGImagePropertyHEICSFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyHEICSDelayTime: CFString

The number of seconds to wait before displaying the next image in the sequence, clamped to a minimum of `0.1` seconds.

let kCGImagePropertyHEICSUnclampedDelayTime: CFString

The unclamped number of seconds to wait before displaying the next image in the sequence.


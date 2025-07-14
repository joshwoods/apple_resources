

- Image I/O
-  kCGImagePropertyWebPUnclampedDelayTime 

Global Variable

# kCGImagePropertyWebPUnclampedDelayTime

The unadjusted number of seconds to wait before displaying the next image in the sequence.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGImagePropertyWebPUnclampedDelayTime: CFString
```

## Discussion

The value of this key is a CFNumber with a floating-point value.

## See Also

### Sequence Timing

let kCGImagePropertyWebPFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyWebPDelayTime: CFString

The number of seconds to wait before displaying the next image in the sequence.

let kCGImagePropertyWebPLoopCount: CFString

The number of times to play the sequence.


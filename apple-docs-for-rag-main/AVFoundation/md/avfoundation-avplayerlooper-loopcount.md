

- AVFoundation
- AVPlayerLooper
-  loopCount 

Instance Property

# loopCount

The number of times the object played the media.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var loopCount: Int { get }
```

## Discussion

This value starts at 0 and increments as the player continues to loop the replica player items.

This property is key-value observable.

## See Also

### Observing Looping State

var status: AVPlayerLooper.Status

A status that indicates the object’s ability to loop playback.

enum Status

Status constants that indicate whether a looper can successfully perform looping playback.


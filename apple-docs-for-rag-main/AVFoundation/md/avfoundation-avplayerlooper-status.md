

- AVFoundation
- AVPlayerLooper
-  status 

Instance Property

# status

A status that indicates the object’s ability to loop playback.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var status: AVPlayerLooper.Status { get }
```

## Discussion

When the value of this property is AVPlayerLooper.Status.failed or AVPlayerLooper.Status.cancelled, you can no longer use the looper for playback. You need to create a new instance to begin looping again.

This property is key-value observable.

## See Also

### Observing Looping State

var loopCount: Int

The number of times the object played the media.

enum Status

Status constants that indicate whether a looper can successfully perform looping playback.


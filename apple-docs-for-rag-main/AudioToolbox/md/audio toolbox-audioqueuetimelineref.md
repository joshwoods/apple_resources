

- Audio Toolbox
-  AudioQueueTimelineRef 

Type Alias

# AudioQueueTimelineRef

Defines an opaque data type that represents an audio queue timeline object.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioQueueTimelineRef = OpaquePointer
```

## Discussion

You can use a timeline object to observe time discontinuities in the audio hardware device associated with an audio queue. A discontinuity is, for example, a period of silence when sound was expected. Causes of discontinuities include changes in device state or data processing overloads. See Technical Q&A 1467, CoreAudio Overload Warnings. You query a timeline object by passing it as a parameter to the AudioQueueGetCurrentTime(_:_:_:_:) function.

## See Also

### Managing the Timeline

func AudioQueueCreateTimeline(AudioQueueRef, UnsafeMutablePointer&lt;AudioQueueTimelineRef?>) -> OSStatus

Creates a timeline object for an audio queue.

func AudioQueueDisposeTimeline(AudioQueueRef, AudioQueueTimelineRef) -> OSStatus

Disposes of an audio queue’s timeline object.

func AudioQueueDeviceGetCurrentTime(AudioQueueRef, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

Gets the current time of the audio hardware device associated with an audio queue.

func AudioQueueDeviceGetNearestStartTime(AudioQueueRef, UnsafeMutablePointer&lt;AudioTimeStamp>, UInt32) -> OSStatus

Gets the start time, for an audio hardware device, that is closest to a requested start time.

func AudioQueueDeviceTranslateTime(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

Converts the time for an audio queue’s associated audio hardware device from one time base representation to another.

func AudioQueueGetCurrentTime(AudioQueueRef, AudioQueueTimelineRef?, UnsafeMutablePointer&lt;AudioTimeStamp>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets the current audio queue time.


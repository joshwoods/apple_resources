

- Audio Toolbox
-  AudioQueueDisposeTimeline(\_:\_:) 

Function

# AudioQueueDisposeTimeline(\_:\_:)

Disposes of an audio queue’s timeline object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueDisposeTimeline(
    _ inAQ: AudioQueueRef,
    _ inTimeline: AudioQueueTimelineRef
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue associated with the timeline object you want to dispose of.

`inTimeline`  

The timeline object to dispose of.

## Return Value

A result code. See Result Codes.

## Discussion

Disposing of an audio queue automatically disposes of any associated resources, including a timeline object. Call this function only if you want to dispose of a timeline object and not the audio queue associated with it.

## See Also

### Related Documentation

func AudioQueueDispose(AudioQueueRef, Bool) -> OSStatus

Disposes of an audio queue.

### Managing the Timeline

func AudioQueueCreateTimeline(AudioQueueRef, UnsafeMutablePointer&lt;AudioQueueTimelineRef?>) -> OSStatus

Creates a timeline object for an audio queue.

func AudioQueueDeviceGetCurrentTime(AudioQueueRef, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

Gets the current time of the audio hardware device associated with an audio queue.

func AudioQueueDeviceGetNearestStartTime(AudioQueueRef, UnsafeMutablePointer&lt;AudioTimeStamp>, UInt32) -> OSStatus

Gets the start time, for an audio hardware device, that is closest to a requested start time.

func AudioQueueDeviceTranslateTime(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

Converts the time for an audio queue’s associated audio hardware device from one time base representation to another.

func AudioQueueGetCurrentTime(AudioQueueRef, AudioQueueTimelineRef?, UnsafeMutablePointer&lt;AudioTimeStamp>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets the current audio queue time.

typealias AudioQueueTimelineRef

Defines an opaque data type that represents an audio queue timeline object.


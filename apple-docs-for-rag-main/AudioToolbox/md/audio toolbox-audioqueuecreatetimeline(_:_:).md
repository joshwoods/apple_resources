

- Audio Toolbox
-  AudioQueueCreateTimeline(\_:\_:) 

Function

# AudioQueueCreateTimeline(\_:\_:)

Creates a timeline object for an audio queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueCreateTimeline(
    _ inAQ: AudioQueueRef,
    _ outTimeline: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue to associate with the new timeline object.

`outTimeline`  

On output, the newly created timeline object.

## Return Value

A result code. See Result Codes.

## Discussion

Create a timeline object if you want to get timeline discontinuity information from an audio queue using the AudioQueueGetCurrentTime(_:_:_:_:) function.

## See Also

### Managing the Timeline

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

typealias AudioQueueTimelineRef

Defines an opaque data type that represents an audio queue timeline object.


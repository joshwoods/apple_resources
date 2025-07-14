

- Audio Toolbox
-  AudioQueueDeviceGetNearestStartTime(\_:\_:\_:) 

Function

# AudioQueueDeviceGetNearestStartTime(\_:\_:\_:)

Gets the start time, for an audio hardware device, that is closest to a requested start time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueDeviceGetNearestStartTime(
    _ inAQ: AudioQueueRef,
    _ ioRequestedStartTime: UnsafeMutablePointer,
    _ inFlags: UInt32
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue whose associated audio hardware device’s start time you want to get.

`ioRequestedStartTime`  

On input, the requested start time. On output, the actual start time.

`inFlags`  

Reserved for future use. Pass `0`.

## Return Value

A result code. See Result Codes.

## Discussion

This function asks an audio queue’s associated device for a start time to use for recording or playback. The time returned will be equal to or later than the requested start time, depending on device and system factors. For example, the start time might be shifted to allow for aligning buffer access. The device must be running to use this function.

## See Also

### Managing the Timeline

func AudioQueueCreateTimeline(AudioQueueRef, UnsafeMutablePointer&lt;AudioQueueTimelineRef?>) -> OSStatus

Creates a timeline object for an audio queue.

func AudioQueueDisposeTimeline(AudioQueueRef, AudioQueueTimelineRef) -> OSStatus

Disposes of an audio queue’s timeline object.

func AudioQueueDeviceGetCurrentTime(AudioQueueRef, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

Gets the current time of the audio hardware device associated with an audio queue.

func AudioQueueDeviceTranslateTime(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

Converts the time for an audio queue’s associated audio hardware device from one time base representation to another.

func AudioQueueGetCurrentTime(AudioQueueRef, AudioQueueTimelineRef?, UnsafeMutablePointer&lt;AudioTimeStamp>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets the current audio queue time.

typealias AudioQueueTimelineRef

Defines an opaque data type that represents an audio queue timeline object.


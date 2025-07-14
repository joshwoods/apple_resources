

- Audio Toolbox
-  AudioQueueDeviceGetCurrentTime(\_:\_:) 

Function

# AudioQueueDeviceGetCurrentTime(\_:\_:)

Gets the current time of the audio hardware device associated with an audio queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueDeviceGetCurrentTime(
    _ inAQ: AudioQueueRef,
    _ outTimeStamp: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue whose associated audio device is to be queried.

`outTimeStamp`  

On output, the current time of the audio hardware device associated with the audio queue. If the device is not running, the only valid field in the audio timestamp structure is `mHostTime`.

## Return Value

A result code. See Result Codes.

## Discussion

This function returns a value whether or not the audio hardware device associated with the audio queue is running. The similar `AudioDeviceGetCurrentTime` function, declared in the `AudioHardware.h` header file, returns an error in this case.

## See Also

### Related Documentation

func AudioDeviceGetCurrentTime(_ inDevice: AudioObjectID, _ outTime: UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

### Managing the Timeline

func AudioQueueCreateTimeline(AudioQueueRef, UnsafeMutablePointer&lt;AudioQueueTimelineRef?>) -> OSStatus

Creates a timeline object for an audio queue.

func AudioQueueDisposeTimeline(AudioQueueRef, AudioQueueTimelineRef) -> OSStatus

Disposes of an audio queue’s timeline object.

func AudioQueueDeviceGetNearestStartTime(AudioQueueRef, UnsafeMutablePointer&lt;AudioTimeStamp>, UInt32) -> OSStatus

Gets the start time, for an audio hardware device, that is closest to a requested start time.

func AudioQueueDeviceTranslateTime(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

Converts the time for an audio queue’s associated audio hardware device from one time base representation to another.

func AudioQueueGetCurrentTime(AudioQueueRef, AudioQueueTimelineRef?, UnsafeMutablePointer&lt;AudioTimeStamp>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets the current audio queue time.

typealias AudioQueueTimelineRef

Defines an opaque data type that represents an audio queue timeline object.


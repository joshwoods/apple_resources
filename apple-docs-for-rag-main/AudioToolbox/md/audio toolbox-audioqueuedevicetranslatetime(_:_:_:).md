

- Audio Toolbox
-  AudioQueueDeviceTranslateTime(\_:\_:\_:) 

Function

# AudioQueueDeviceTranslateTime(\_:\_:\_:)

Converts the time for an audio queue’s associated audio hardware device from one time base representation to another.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueDeviceTranslateTime(
    _ inAQ: AudioQueueRef,
    _ inTime: UnsafePointer,
    _ outTime: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue associated with the device whose times are being translated.

`inTime`  

The time to be translated.

`outTime`  

On output, the translated time.

## Return Value

A result code. See Result Codes.

## Discussion

The device must be running for this function to provide a result. For an explanation of the various time base representations for an audio hardware device, see AudioTimeStamp in Core Audio Data Types.

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

func AudioQueueGetCurrentTime(AudioQueueRef, AudioQueueTimelineRef?, UnsafeMutablePointer&lt;AudioTimeStamp>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets the current audio queue time.

typealias AudioQueueTimelineRef

Defines an opaque data type that represents an audio queue timeline object.


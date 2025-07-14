

- Core Media
-  CMAudioClockCreate(allocator:clockOut:) 

Function

# CMAudioClockCreate(allocator:clockOut:)

Creates a clock that advances at the same rate as audio output.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMAudioClockCreate(
    allocator: CFAllocator?,
    clockOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator for the new clock; pass kCFAllocatorDefault or `nil` to use the default allocator.

`clockOut`  

Upon return, a pointer to the newly created clock.

## Discussion

This clock doesn’t drift from audio output, but may drift from CMClockGetHostTimeClock(). When audio output is completely stopped, the clock continues to advance, tracking `CMClockGetHostTimeClock` until audio output starts up again.

Important

In Objective-C, you’re responsible for calling CFRelease to release the returned `clockOut`.

You can use this clock as the sourceClock of an AVPlayer instance when synchronizing video-only playback with audio played through other APIs or objects.

Note

For Mac apps built with Mac Catalyst, use CMAudioDeviceClockCreate(allocator:deviceUID:clockOut:) or CMAudioDeviceClockCreateFromAudioDeviceID(allocator:deviceID:clockOut:) to target a specific, nondefault audio device.

## See Also

### Creating Audio Clocks

func CMAudioDeviceClockCreate(allocator: CFAllocator?, deviceUID: CFString?, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that tracks playback through a Core Audio device with the specified unique identifier.

func CMAudioDeviceClockCreateFromAudioDeviceID(allocator: CFAllocator?, deviceID: AudioDeviceID, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that tracks playback through a Core Audio device with the specified identifier.


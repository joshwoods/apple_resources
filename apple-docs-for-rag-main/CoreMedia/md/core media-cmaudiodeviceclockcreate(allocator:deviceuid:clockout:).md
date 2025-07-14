

- Core Media
-  CMAudioDeviceClockCreate(allocator:deviceUID:clockOut:) 

Function

# CMAudioDeviceClockCreate(allocator:deviceUID:clockOut:)

Creates a clock that tracks playback through a Core Audio device with the specified unique identifier.

macOS 10.8+

``` source
func CMAudioDeviceClockCreate(
    allocator: CFAllocator?,
    deviceUID: CFString?,
    clockOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator for the new clock; pass kCFAllocatorDefault or `NULL` to use the default allocator.

`deviceUID`  

The unique ID of the device for which to create a clock. Pass `NULL` to create a clock that tracks the default device.

`clockOut`  

Upon return, a pointer to the newly created clock.

## Discussion

When the associated device is completely stopped, the clock continues to advance, tracking CMClockGetHostTimeClock() until the audio device starts up again.

Important

In Objective-C, you’re responsible for calling CFRelease to release the returned `clockOut`.

## See Also

### Creating Audio Clocks

func CMAudioClockCreate(allocator: CFAllocator?, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that advances at the same rate as audio output.

func CMAudioDeviceClockCreateFromAudioDeviceID(allocator: CFAllocator?, deviceID: AudioDeviceID, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that tracks playback through a Core Audio device with the specified identifier.




- Core Media
-  CMAudioDeviceClockCreateFromAudioDeviceID(allocator:deviceID:clockOut:) 

Function

# CMAudioDeviceClockCreateFromAudioDeviceID(allocator:deviceID:clockOut:)

Creates a clock that tracks playback through a Core Audio device with the specified identifier.

macOS 10.8+

``` source
func CMAudioDeviceClockCreateFromAudioDeviceID(
    allocator: CFAllocator?,
    deviceID: AudioDeviceID,
    clockOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator for the new clock; pass kCFAllocatorDefault or `NULL` to use the default allocator.

`deviceID`  

The AudioDeviceID of the device for which to create a clock.

`clockOut`  

Upon return, a pointer to the newly created clock.

## Overview

Important

In Objective-C, you’re responsible for calling CFRelease to release the clock returned in `clockOut`.

## See Also

### Creating Audio Clocks

func CMAudioClockCreate(allocator: CFAllocator?, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that advances at the same rate as audio output.

func CMAudioDeviceClockCreate(allocator: CFAllocator?, deviceUID: CFString?, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that tracks playback through a Core Audio device with the specified unique identifier.


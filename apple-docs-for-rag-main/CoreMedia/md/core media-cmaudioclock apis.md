

- Core Media
-  CMAudioClock APIs 

API Collection

# CMAudioClock APIs

A specialized reference clock that synchronizes with audio sources.

## Overview

An audio clock is a specialized CMClock that you use to synchronize with audio sources. For details on clocks and synchronization, see CMClock.

## Topics

### Creating Audio Clocks

func CMAudioClockCreate(allocator: CFAllocator?, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that advances at the same rate as audio output.

func CMAudioDeviceClockCreate(allocator: CFAllocator?, deviceUID: CFString?, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that tracks playback through a Core Audio device with the specified unique identifier.

func CMAudioDeviceClockCreateFromAudioDeviceID(allocator: CFAllocator?, deviceID: AudioDeviceID, clockOut: UnsafeMutablePointer&lt;CMClock?>) -> OSStatus

Creates a clock that tracks playback through a Core Audio device with the specified identifier.

### Configuring Audio Clocks

func CMAudioDeviceClockGetAudioDevice(CMClock, deviceUIDOut: AutoreleasingUnsafeMutablePointer&lt;CFString?>?, deviceIDOut: UnsafeMutablePointer&lt;AudioDeviceID>?, trackingDefaultDeviceOut: UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Returns the Core Audio device the clock is tracking.

func CMAudioDeviceClockSetAudioDeviceUID(CMClock, deviceUID: CFString?) -> OSStatus

Changes the Core Audio device the clock is tracking by specifying a new device unique identifier.

func CMAudioDeviceClockSetAudioDeviceID(CMClock, deviceID: AudioDeviceID) -> OSStatus

Changes the Core Audio device the clock is tracking by specifying a new device identifier.

## See Also

### Media Synchronization

CMClock APIs

A reference clock you use to synchronize applications and devices.

CMTimebase APIs

A model of a timeline under application control.


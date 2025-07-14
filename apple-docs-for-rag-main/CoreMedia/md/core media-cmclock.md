

- Core Media
-  CMClock 

Class

# CMClock

An object that represents a source of time.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
class CMClock
```

## Overview

A clock represents a source of time information: a piece of hardware that measures the passage of time. One example of a clock is the host time clock, accessible via CMClockGetHostTimeClock(). It measures time using the CPU system clock, which in macOS is `mach_absolute_time()`. Every audio device is also a clock because the audio samples that it outputs or inputs each have a defined duration (for example, 1/48000 of a second for 48 kHz audio).

`CMClocks` are read-only; they cannot be stopped or started, and the current time cannot be set. A `CMClock` has one primary function, CMClockGetTime(_:), which tells what time it is now. Additionally, the `CMSync` infrastructure monitors relative drift between `CMClocks`.

## Topics

### Inspecting a Clock

var time: CMTime

The current time.

static var typeID: CFTypeID

The Core Foundation identifier that corresponds to the clock structure.

### Stopping a Clock

func invalidate()

Stops the clock.

### Getting the Host Time

static var hostTimeClock: CMClock

The singleton clock that the system identifies as host time.

### Getting Time and Devices

func anchorTime() throws -> (anchorTime: CMTime, referenceTime: CMTime)

Returns the current time from a clock and the matching time from the clock’s reference clock.

func audioDevice() throws -> (deviceUID: String?, deviceID: AudioDeviceID, trackingDefaultDevice: Bool)

Returns the audio device the clock tracks.

func setAudioDeviceID(AudioDeviceID) throws

Sets the audio device by using the device identifier.

func setAudioDeviceUID(String?) throws

Sets the audio device by using the unique device identifier.

### Determining Time Drift

func mightDrift(relativeTo: CMClock) -> Bool

Returns a Boolean value that indicates whether it’s possible for one timebase or clock to drift relative to another.

### Converting Time

static func convertHostTimeToSystemUnits(CMTime) -> UInt64

Converts a host time from a time structure to the host time’s native units.

static func convertSystemUnitsToHostTime(UInt64) -> CMTime

Converts a host time from native units to a time structure.

### Constants

struct Error

Constants that describe clock errors.

### Default Implementations

CMSyncProtocol Implementations

## Relationships

### Conforms To

- CMSyncProtocol
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Data Types

typealias CMClockOrTimebase

A type you use in argument lists and function results to indicate that you can pass either a clock or timebase.

func CMClockGetTypeID() -> CFTypeID

Returns the core foundation type identifier of a clock type.


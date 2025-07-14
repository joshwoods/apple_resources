

- Core Media
-  CMClock APIs 

API Collection

# CMClock APIs

A reference clock you use to synchronize applications and devices.

## Overview

`The CMSync` API provides a reference clock that you use to synchronize applications and devices. This API also provides functions to monitor relative drift between `CMClocks` and functions that are associated with timer services.

## Topics

### Accessing the Host Clock

func CMClockGetHostTimeClock() -> CMClock

Returns a reference to the singleton clock that reflects the host time.

### Stopping the Clock

func CMClockInvalidate(CMClock)

Stops the clock.

### Accessing and Converting Time

func CMClockGetTime(CMClock) -> CMTime

Returns the current time from a clock.

func CMClockGetAnchorTime(CMClock, clockTimeOut: UnsafeMutablePointer&lt;CMTime>, referenceClockTimeOut: UnsafeMutablePointer&lt;CMTime>) -> OSStatus

Returns the current time from a clock and the matching time from the clock’s reference clock.

func CMClockConvertHostTimeToSystemUnits(CMTime) -> UInt64

Converts a host time from a core media time structure to the host time’s native units.

func CMClockMakeHostTimeFromSystemUnits(UInt64) -> CMTime

Converts a host time from native units to a core media time structure.

### Getting and Syncing Time

func CMSyncGetTime(CMClockOrTimebase) -> CMTime

Returns the time from a clock or timebase.

func CMSyncGetRelativeRate(CMClockOrTimebase, relativeTo: CMClockOrTimebase) -> Float64

Returns the relative rate of one timebase or clock relative to another timebase or clock.

func CMSyncGetRelativeRateAndAnchorTime(CMClockOrTimebase, relativeTo: CMClockOrTimebase, relativeRateOut: UnsafeMutablePointer&lt;Float64>?, anchorTimeOut: UnsafeMutablePointer&lt;CMTime>?, relativeToAnchorTimeOut: UnsafeMutablePointer&lt;CMTime>?) -> OSStatus

Returns the relative rate of one timebase or clock relative to another timebase or clock and the times of each timebase or clock at which the relative rate went into effect.

func CMSyncConvertTime(CMTime, from: CMClockOrTimebase, to: CMClockOrTimebase) -> CMTime

Converts a time from one timebase or clock to another timebase or clock.

### Determining Clock Drift

func CMClockMightDrift(CMClock, otherClock: CMClock) -> Bool

Returns a Boolean value that indicates whether it’s possible for two clocks to drift relative to each other.

func CMSyncMightDrift(CMClockOrTimebase, CMClockOrTimebase) -> Bool

Returns a Boolean value that indicates whether it’s possible for one timebase or clock to drift relative to the other.

### Data Types

class CMClock

An object that represents a source of time.

typealias CMClockOrTimebase

A type you use in argument lists and function results to indicate that you can pass either a clock or timebase.

func CMClockGetTypeID() -> CFTypeID

Returns the core foundation type identifier of a clock type.

### Constants

CMClock Error Codes

Constants that represent the errors in Core Media clock operations.

CMTimebase Error Codes

Constants that represent errors in Core Media timebase operations.

CMSync error codes

Constants that represent error codes Core Media sync operations return.

Timebase Notifications

Keys that represent timebase notifications.

## See Also

### Media Synchronization

CMAudioClock APIs

A specialized reference clock that synchronizes with audio sources.

CMTimebase APIs

A model of a timeline under application control.


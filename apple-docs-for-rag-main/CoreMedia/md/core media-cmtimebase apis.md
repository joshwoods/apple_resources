

- Core Media
-  CMTimebase APIs 

API Collection

# CMTimebase APIs

A model of a timeline under application control.

## Overview

A timebase represents a timeline that clients can control by setting the rate and time. Each timebase has either a host clock or a host timebase, and its rate is expressed relative to its host:

- When a timebase has rate 0.0, its time is fixed and doesn’t change as its host’s time changes.

- When a timebase has rate 1.0, its time increases one second as its host’s time increases by one second.

- When a timebase has rate 2.0, its time increases two seconds as its host’s time increases by one second.

- When a timebase has rate -1.0, its time decreases one second as its host’s time increases by one second.

If a timebase has a host timebase, the host timebase’s rate is a factor in determining the timebase’s effective rate. In fact, a timebase’s effective rate is defined as the product of its rate, its host timebase’s rate, its host timebase’s host timebase’s rate, and so on up to the ultimate host clock. This is the rate at which the timebase’s time changes relative to the ultimate host clock.

## Topics

### Creating Timebases

func CMTimebaseCreateWithSourceClock(allocator: CFAllocator?, sourceClock: CMClock, timebaseOut: UnsafeMutablePointer&lt;CMTimebase?>) -> OSStatus

Creates a timebase by using a source clock.

func CMTimebaseCreateWithSourceTimebase(allocator: CFAllocator?, sourceTimebase: CMTimebase, timebaseOut: UnsafeMutablePointer&lt;CMTimebase?>) -> OSStatus

Creates a timebase by using a source timebase.

### Copying Timebases

func CMTimebaseCopySource(CMTimebase) -> CMClockOrTimebase

Returns the immediate source — either a clock or timebase — of a timebase.

func CMTimebaseCopySourceClock(CMTimebase) -> CMClock?

Returns the immediate source clock of a timebase.

func CMTimebaseCopySourceTimebase(CMTimebase) -> CMTimebase?

Returns the immediate source timebase of a timebase.

func CMTimebaseCopyUltimateSourceClock(CMTimebase) -> CMClock

Returns the source clock that’s the source of all of a timebase’s source timebases.

### Getting and Setting Time

func CMTimebaseGetTime(CMTimebase) -> CMTime

Returns the current time from a timebase.

func CMTimebaseGetTimeWithTimeScale(CMTimebase, timescale: CMTimeScale, method: CMTimeRoundingMethod) -> CMTime

Returns the current time from a timebase in the specified timescale.

func CMTimebaseGetTimeAndRate(CMTimebase, timeOut: UnsafeMutablePointer&lt;CMTime>?, rateOut: UnsafeMutablePointer&lt;Float64>?) -> OSStatus

Returns the current time and rate of a timebase.

func CMTimebaseSetTime(CMTimebase, time: CMTime) -> OSStatus

Sets the current time of a timebase.

func CMTimebaseSetSourceClock(CMTimebase, CMClock) -> OSStatus

Sets the source clock of a timebase.

func CMTimebaseSetSourceTimebase(CMTimebase, CMTimebase) -> OSStatus

Sets the source timebase of a timebase.

func CMTimebaseSetAnchorTime(CMTimebase, timebaseTime: CMTime, immediateSourceTime: CMTime) -> OSStatus

Sets the time of a timebase at a particular host time.

### Getting and Setting the Time Rate

func CMTimebaseGetRate(CMTimebase) -> Float64

Returns the current rate of a timebase.

func CMTimebaseGetEffectiveRate(CMTimebase) -> Float64

Returns the effective rate of a timebase, which combines its rate with the rates of all its host timebases.

func CMTimebaseSetRate(CMTimebase, rate: Float64) -> OSStatus

Sets the rate of a timebase.

func CMTimebaseSetRateAndAnchorTime(CMTimebase, rate: Float64, anchorTime: CMTime, immediateSourceTime: CMTime) -> OSStatus

Sets the time of a timebase at a particular host time, and changes the rate at exactly that time.

### Interacting with Timers

func CMTimebaseAddTimer(CMTimebase, timer: CFRunLoopTimer, runloop: CFRunLoop) -> OSStatus

Adds the timer to the list of timers the timebase manages.

func CMTimebaseAddTimerDispatchSource(CMTimebase, timerSource: dispatch_source_t) -> OSStatus

Adds the timer dispatch source to the list of timers the timebase manages.

func CMTimebaseRemoveTimer(CMTimebase, timer: CFRunLoopTimer) -> OSStatus

Removes the timer from the list of timers the timebase manages.

func CMTimebaseRemoveTimerDispatchSource(CMTimebase, timerSource: dispatch_source_t) -> OSStatus

Removes the timer dispatch source from the list of timers the timebase manages.

func CMTimebaseSetTimerNextFireTime(CMTimebase, timer: CFRunLoopTimer, fireTime: CMTime, flags: UInt32) -> OSStatus

Sets the time on the timebase’s timeline at which the timer should fire next.

func CMTimebaseSetTimerToFireImmediately(CMTimebase, timer: CFRunLoopTimer) -> OSStatus

Sets the timer to fire immediately once, overriding any previous timer calls.

func CMTimebaseSetTimerDispatchSourceNextFireTime(CMTimebase, timerSource: dispatch_source_t, fireTime: CMTime, flags: UInt32) -> OSStatus

Sets the time on the timebase’s timeline at which the timer dispatch source should fire next.

func CMTimebaseSetTimerDispatchSourceToFireImmediately(CMTimebase, timerSource: dispatch_source_t) -> OSStatus

Sets the timer dispatch source to fire immediately once, overriding any previous timer call.

### Pausing Time Notifications

func CMTimebaseNotificationBarrier(CMTimebase) -> OSStatus

Requests that the timebase wait until it isn’t posting notifications.

### Data Types

class CMTimebase

A model of a timeline under application control.

struct CMSync

A type that represents time syncing.

protocol CMSyncProtocol

A type that provides behavior for syncing time.

### Timebase Errors

var kCMTimebaseError_MissingRequiredParameter: OSStatus

A timebase error that indicates a parameter is missing.

var kCMTimebaseError_InvalidParameter: OSStatus

A timebase error that indicates a parameter isn’t valid.

var kCMTimebaseError_AllocationFailed: OSStatus

A timebase error that indicates the memory allocation fails.

var kCMTimebaseError_TimerIntervalTooShort: OSStatus

A timebase error that indicates the time interval is too short.

var kCMTimebaseError_ReadOnly: OSStatus

A timebase error that indicates the system attempts to modify a read-only timebase.

### Constants

func CMTimebaseGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier that identifies a timebase object.

### Notifications

let kCMTimebaseNotificationKey_EventTime: CFString

A notification that a timebase posts after a discontinuous time jump.

### Deprecations

func CMTimebaseSetRateAndAnchorTime(CMTimebase, rate: Double, anchorTime: CMTime, immediateMasterTime: CMTime)Deprecated

func CMTimebaseGetMasterTimebase(CMTimebase) -> CMTimebase?

Returns the immediate host timebase of a timebase.

Deprecated

func CMTimebaseGetMasterClock(CMTimebase) -> CMClock?

Returns the immediate host clock of a timebase.

Deprecated

func CMTimebaseGetMaster(CMTimebase) -> CMClockOrTimebase?

Returns the immediate host (either timebase or clock) of a timebase.

Deprecated

func CMTimebaseGetUltimateMasterClock(CMTimebase) -> CMClock?

Returns the host clock that is the host of all of a timebase’s host timebases.

Deprecated

func CMTimebaseSetMasterClock(CMTimebase, CMClock) -> OSStatus

Sets the time of a timebase at a particular source time.

Deprecated

func CMTimebaseSetMasterTimebase(CMTimebase, CMTimebase) -> OSStatusDeprecated

func CMTimebaseSetAnchorTime(CMTimebase, timebaseTime: CMTime, immediateMasterTime: CMTime)

Sets the time of a timebase at a particular source time.

Deprecated

func CMTimebaseCopyMaster(CMTimebase) -> CMClockOrTimebase

Returns the immediate host timebase of a timebase.

Deprecated

func CMTimebaseCopyMasterClock(CMTimebase) -> CMClock?

Returns the immediate host clock of a timebase.

Deprecated

func CMTimebaseCopyMasterTimebase(CMTimebase) -> CMTimebase?

Returns the immediate host timebase of a timebase.

Deprecated

func CMTimebaseCopyUltimateMasterClock(CMTimebase) -> CMClock

Returns the host clock that is the host of all of a timebase’s host timebases.

Deprecated

func CMTimebaseCreateWithMasterClock(allocator: CFAllocator?, masterClock: CMClock, timebaseOut: UnsafeMutablePointer&lt;CMTimebase?>) -> OSStatus

Creates a timebase by using a primary clock.

Deprecated

func CMTimebaseCreateWithMasterTimebase(allocator: CFAllocator?, masterTimebase: CMTimebase, timebaseOut: UnsafeMutablePointer&lt;CMTimebase?>) -> OSStatus

Creates a timebase by using a host timebase.

Deprecated

## See Also

### Media Synchronization

CMClock APIs

A reference clock you use to synchronize applications and devices.

CMAudioClock APIs

A specialized reference clock that synchronizes with audio sources.


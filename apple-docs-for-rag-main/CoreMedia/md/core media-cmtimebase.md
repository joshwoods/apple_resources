

- Core Media
-  CMTimebase 

Class

# CMTimebase

A model of a timeline under application control.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
class CMTimebase
```

## Topics

### Timebases

static let farFuture: CFAbsoluteTime

A time far into the future that represents the year 2257.

static let veryLongTimeInterval: CFTimeInterval

A time far into the future that represents 256 years.

### Inspecting Timebases

var time: CMTime

The current time.

var rate: Double

The current rate relative to its immediate primary clock or timebase.

var source: any CMSyncProtocol

The immediate source that represents the clock or timebase.

var sourceClock: CMClock?

Returns the immediate source clock, if any.

var sourceTimebase: CMTimebase?

Returns the immediate source timebase, if any.

var effectiveRate: Double

The effective rate that combines its rate with the rates of all its primary timebases.

var timeAndRate: (time: CMTime, rate: Double)

Returns the current time and rate.

var ultimateSourceClock: CMClock

Returns the source clock that’s the source of all the other source timebases.

### Adding and Removing Timers

func addTimer(Timer, on: RunLoop) throws

Adds the timer to the list of timers the timebase manages.

func addTimer&lt;T>(T) throws

Adds the timer dispatch source to the list of timers the timebase manages.

func removeTimer(Timer) throws

Removes the timer from the list of timers the timebase manages.

func removeTimer&lt;T>(T) throws

Removes the timer dispatch source from the list of timers the timebase manages.

### Getting and Setting Time

func setTime(CMTime) throws

Sets the current time.

func time(withTimescale: CMTimeScale, rounding: CMTimeRoundingMethod) -> CMTime

Returns the current time in the timescale you request.

### Getting and Setting the Timebase Rate

func setRate(Double) throws

Sets the rate.

func setRateAndAnchorTime(rate: Double, anchorTime: CMTime, referenceTime: CMTime) throws

Sets the time at a particular primary time, and changes the rate at exactly that time.

### Setting Timers

func setTimerNextFireTime(Timer, fireTime: CMTime) throws

Sets the time on the timebase’s timeline at which the timer should fire next.

func setTimerNextFireTime&lt;T>(T, fireTime: CMTime) throws

Sets the time on the timebase’s timeline at which the timer dispatch source should fire next.

func setTimerToFireImmediately(Timer) throws

Sets the timer to fire immediately once, overriding any previous calls.

func setTimerToFireImmediately&lt;T>(T) throws

Sets the timer dispatch source to fire immediately once, overriding any previous calls.

### Pausing Time Notifications

func notificationBarrier() throws

Requests that the timebase wait until it isn’t posting notifications.

### Setting the Anchor Time

func setAnchorTime(CMTime, referenceTime: CMTime) throws

Sets the time at a particular source time.

### Notifications

static let effectiveRateChanged: NSNotification.Name

A notification that posts by a timebase after the effective rate changes.

static let timeJumped: NSNotification.Name

A notification that posts by a timebase after a discontinuous time jump.

### Constants

struct Error

Constants that describe timebase errors.

struct NotificationKey

Constants that describe notification keys.

static var typeID: CFTypeID

A Core Foundation type identifier that represents a timebase object.

### Deprecations

var master: any CMSyncProtocol

var masterClock: CMClock?

var masterTimebase: CMTimebase?

var ultimateMasterClock: CMClock

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

struct CMSync

A type that represents time syncing.

protocol CMSyncProtocol

A type that provides behavior for syncing time.


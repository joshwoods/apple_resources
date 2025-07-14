

- Kernel
- Hardware Families
- ATA
-  ATATimerEventSource 

Class

# ATATimerEventSource

Extend the timer event source to allow checking for timer expiration from behind the workloop.

macOS 10.0+

``` source
class ATATimerEventSource : IOTimerEventSource
```

## Topics

### Miscellaneous

ataTimerEventSource

allocate an instance of this type.

cancelTimeout

overrides in order to set/clear the timed out flag

disable

overrides in order to set/clear the timed out flag

enable

overrides in order to set/clear the timed out flag

hasTimedOut

returns true if the timer has expired since the last enable/disable or setTimeout() or wakeAtTime() call.

init

myTimeout

my timeout function which sets the timedOut flag atomically.

setTimeoutFunc

override to install my timeout function instead of the super's.

wakeAtTime

overrides in order to set/clear the timed out flag

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- cancelTimeout

- disable

- enable

- getMetaClass

- hasTimedOut

- init

- setTimeoutFunc

- wakeAtTime

### Type Methods

+ ataTimerEventSource

+ myTimeout

## Relationships

### Inherits From

- IOTimerEventSource


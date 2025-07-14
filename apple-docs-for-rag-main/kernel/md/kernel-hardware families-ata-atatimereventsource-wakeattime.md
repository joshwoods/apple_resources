

- Kernel
- Hardware Families
- ATA
- ATATimerEventSource
-  wakeAtTime 

# wakeAtTime

overrides in order to set/clear the timed out flag

``` source
virtual IOReturn wakeAtTime(
 UnsignedWide abstime); 
```

## See Also

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


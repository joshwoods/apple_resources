

- Core Media
-  CMTimebaseSetAnchorTime(\_:timebaseTime:immediateMasterTime:) Deprecated

Function

# CMTimebaseSetAnchorTime(\_:timebaseTime:immediateMasterTime:)

Sets the time of a timebase at a particular source time.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac CatalystmacOS 10.8–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOSwatchOS 6.0–8.0Deprecated

``` source
func CMTimebaseSetAnchorTime(
    _ timebase: CMTimebase,
    timebaseTime: CMTime,
    immediateMasterTime: CMTime
)
```

Deprecated

Use CMTimebaseSetAnchorTime(_:timebaseTime:immediateSourceTime:) instead.

## See Also

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


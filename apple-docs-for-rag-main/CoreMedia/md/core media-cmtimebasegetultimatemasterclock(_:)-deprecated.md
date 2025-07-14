

- Core Media
-  CMTimebaseGetUltimateMasterClock(\_:) Deprecated

Function

# CMTimebaseGetUltimateMasterClock(\_:)

Returns the host clock that is the host of all of a timebase’s host timebases.

iOS 6.0–9.0DeprecatediPadOS 6.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func CMTimebaseGetUltimateMasterClock(_ timebase: CMTimebase) -> CMClock?
```

Deprecated

Use CMTimebaseCopyUltimateSourceClock(_:) instead.

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


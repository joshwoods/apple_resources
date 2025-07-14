

- Core Media
-  CMTimebaseCreateWithSourceClock(allocator:sourceClock:timebaseOut:) 

Function

# CMTimebaseCreateWithSourceClock(allocator:sourceClock:timebaseOut:)

Creates a timebase by using a source clock.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseCreateWithSourceClock(
    allocator: CFAllocator?,
    sourceClock: CMClock,
    timebaseOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for creating the timebase.

`sourceClock`  

The source clock.

`timebaseOut`  

Receives the timebase the function creates.

## See Also

### Creating Timebases

func CMTimebaseCreateWithSourceTimebase(allocator: CFAllocator?, sourceTimebase: CMTimebase, timebaseOut: UnsafeMutablePointer&lt;CMTimebase?>) -> OSStatus

Creates a timebase by using a source timebase.


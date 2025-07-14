

- Core Media
-  CMTimebaseCreateWithSourceTimebase(allocator:sourceTimebase:timebaseOut:) 

Function

# CMTimebaseCreateWithSourceTimebase(allocator:sourceTimebase:timebaseOut:)

Creates a timebase by using a source timebase.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseCreateWithSourceTimebase(
    allocator: CFAllocator?,
    sourceTimebase: CMTimebase,
    timebaseOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for creating the timebase.

`sourceTimebase`  

The source timebase.

`timebaseOut`  

Receives the timebase the function creates.

## See Also

### Creating Timebases

func CMTimebaseCreateWithSourceClock(allocator: CFAllocator?, sourceClock: CMClock, timebaseOut: UnsafeMutablePointer&lt;CMTimebase?>) -> OSStatus

Creates a timebase by using a source clock.


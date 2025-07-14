

- Core Media
-  CMClockInvalidate(\_:) 

Function

# CMClockInvalidate(\_:)

Stops the clock.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClockInvalidate(_ clock: CMClock)
```

## Parameters 

`clock`  

The clock to stop.

## Discussion

After invalidation, the clock returns errors from all APIs. Only the owner of the clock should call this function.


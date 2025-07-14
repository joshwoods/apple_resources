

- AVFoundation
- AVPlayer
-  seek(to:toleranceBefore:toleranceAfter:) 

Instance Method

# seek(to:toleranceBefore:toleranceAfter:)

Requests that the player seek to a specified time with the amount of accuracy specified by the time tolerance values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func seek(
    to time: CMTime,
    toleranceBefore: CMTime,
    toleranceAfter: CMTime
)
```

## Parameters 

`time`  

A time to seek to.

`toleranceBefore`  

A tolerance before the target time to allow.

`toleranceAfter`  

A tolerance after the target time to allow.

## Mentioned in 

Controlling the transport behavior of a player

## Discussion

The player seeks within the range `[time-beforeTolerance, time+afterTolerance]`, and may differ from the specified time for efficiency. You can request sample accurate seeking by passing a time value of`kCMTimeZero` for both `toleranceBefore` and `toleranceAfter`. Sample accurate seeking may incur additional decoding delay which can impact seeking performance.

Passing `kCMTimePositiveInfinity` for both `toleranceBefore` and `toleranceAfter` is the same as messaging seek(to:) directly.

## See Also

### Seeking Through Media

func seek(to: CMTime)

Requests that the player seek to a specified time.

func seek(to: CMTime, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified time, and to notify you when the seek is complete.

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified time with the amount of accuracy specified by the time tolerance values, and to notify you when the seek is complete.

func seek(to: Date)

Requests that the player seek to a specified date.

func seek(to: Date, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified date, and to notify you when the seek is complete.




- AVFoundation
- AVPlayer
-  seek(to:) 

Instance Method

# seek(to:)

Requests that the player seek to a specified date.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func seek(to date: Date)
```

## Parameters 

`date`  

The time to which to seek.

## Discussion

The time to which the player seeks may differ from the specified `date` for efficiency. For sample accurate seeking see seek(to:toleranceBefore:toleranceAfter:).

## See Also

### Seeking Through Media

func seek(to: CMTime)

Requests that the player seek to a specified time.

func seek(to: CMTime, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified time, and to notify you when the seek is complete.

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime)

Requests that the player seek to a specified time with the amount of accuracy specified by the time tolerance values.

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified time with the amount of accuracy specified by the time tolerance values, and to notify you when the seek is complete.

func seek(to: Date, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified date, and to notify you when the seek is complete.


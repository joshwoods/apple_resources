

- AVFoundation
- AVPlayer
-  seek(to:) 

Instance Method

# seek(to:)

Requests that the player seek to a specified time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func seek(to time: CMTime)
```

## Parameters 

`time`  

The time to which to seek.

## Mentioned in 

Controlling the transport behavior of a player

Presenting Chapter Markers

## Discussion

The time to which the player seeks may differ from the specified requested time for efficiency. For sample accurate seeking see seek(to:toleranceBefore:toleranceAfter:).

## See Also

### Seeking Through Media

func seek(to: CMTime, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified time, and to notify you when the seek is complete.

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime)

Requests that the player seek to a specified time with the amount of accuracy specified by the time tolerance values.

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified time with the amount of accuracy specified by the time tolerance values, and to notify you when the seek is complete.

func seek(to: Date)

Requests that the player seek to a specified date.

func seek(to: Date, completionHandler: (Bool) -> Void)

Requests that the player seek to a specified date, and to notify you when the seek is complete.


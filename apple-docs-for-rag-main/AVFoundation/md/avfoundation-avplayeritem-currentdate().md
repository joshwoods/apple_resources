

- AVFoundation
- AVPlayerItem
-  currentDate() 

Instance Method

# currentDate()

Returns the current time of the item as a date.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func currentDate() -> Date?
```

## Return Value

The current time of the item as a date, or `nil` if there isn’t a mapped date for the item.

## Discussion

The system calculates this value from the `EXT-X-PROGRAM-DATE-TIME` tag.

## See Also

### Accessing Timing Information

func currentTime() -> CMTime

Returns the current time of the item.

var duration: CMTime

The duration of the item.

var timebase: CMTimebase?

The timebase information for the item.


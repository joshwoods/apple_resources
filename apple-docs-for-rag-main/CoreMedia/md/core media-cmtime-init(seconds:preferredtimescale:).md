

- Core Media
- CMTime
-  init(seconds:preferredTimescale:) 

Initializer

# init(seconds:preferredTimescale:)

Creates a time that represents number of seconds in a preferred timescale.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    seconds: Double,
    preferredTimescale: CMTimeScale
)
```

## Parameters 

`seconds`  

The number of seconds to represent.

`preferredTimescale`  

The preferred timescale of the time.

## Discussion

Specify a positive preferred timescale value, or the resulting time is invalid.

If you specify a value that causes an overflow, the system repeatedly halves the value until the overflow goes away or the timescale equals `1`. If the value still overflows at that point, the system sets the value to positive or negative infinity.

Query the hasBeenRounded property value to determine whether the value, when converted back to seconds, precisely matches the original seconds value.

## See Also

### Creating a Time

init(value: CMTimeValue, timescale: CMTimeScale)

Creates a time with a value and timescale.

init(value: CMTimeValue, timescale: CMTimeScale, flags: CMTimeFlags, epoch: CMTimeEpoch)

Creates a time with a value, timescale, flags, and epoch.

init()

Creates a time with an invalid value.




- Core Media
- CMTime
-  init() 

Initializer

# init()

Creates a time with an invalid value.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
init()
```

## Discussion

Using this initializer creates a time equal to invalid.

## See Also

### Creating a Time

init(value: CMTimeValue, timescale: CMTimeScale)

Creates a time with a value and timescale.

init(value: CMTimeValue, timescale: CMTimeScale, flags: CMTimeFlags, epoch: CMTimeEpoch)

Creates a time with a value, timescale, flags, and epoch.

init(seconds: Double, preferredTimescale: CMTimeScale)

Creates a time that represents number of seconds in a preferred timescale.


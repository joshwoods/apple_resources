

- Core Media
- CMTime
-  init(value:timescale:flags:epoch:) 

Initializer

# init(value:timescale:flags:epoch:)

Creates a time with a value, timescale, flags, and epoch.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    value: CMTimeValue,
    timescale: CMTimeScale,
    flags: CMTimeFlags,
    epoch: CMTimeEpoch
)
```

## Parameters 

`value`  

An integer time value.

`timescale`  

An integer timescale value.

`flags`  

Optional flags to specify for the time.

`epoch`  

An epoch for the time, which is typically `0`.

## See Also

### Creating a Time

init(value: CMTimeValue, timescale: CMTimeScale)

Creates a time with a value and timescale.

init(seconds: Double, preferredTimescale: CMTimeScale)

Creates a time that represents number of seconds in a preferred timescale.

init()

Creates a time with an invalid value.


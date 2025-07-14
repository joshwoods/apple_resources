

- Core Media
- CMTimebase
-  time(withTimescale:rounding:) 

Instance Method

# time(withTimescale:rounding:)

Returns the current time in the timescale you request.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func time(
    withTimescale timescale: CMTimeScale,
    rounding: CMTimeRoundingMethod = .`default`
) -> CMTime
```

## See Also

### Getting and Setting Time

func setTime(CMTime) throws

Sets the current time.


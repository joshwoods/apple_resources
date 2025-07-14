

- Core Media
- CMSyncProtocol
-  convertTime(\_:to:) 

Instance Method

# convertTime(\_:to:)

Converts a time from one timebase or clock to another timebase or clock.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func convertTime(
    _ time: CMTime,
    to clockOrTimebase: T
) -> CMTime where T : CMSyncProtocol
```

**Required**

## Parameters 

`time`  

The time to convert from.

`clockOrTimebase`  

The clock or time to convert to.


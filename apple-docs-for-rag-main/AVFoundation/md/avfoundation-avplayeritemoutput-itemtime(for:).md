

- AVFoundation
- AVPlayerItemOutput
-  itemTime(for:) 

Instance Method

# itemTime(for:)

Converts a Core Video timestamp to the item’s timebase.

macOS 10.8+

``` source
func itemTime(for timestamp: CVTimeStamp) -> CMTime
```

## Parameters 

`timestamp`  

A timestamp value provided by the Core Video framework.

## Return Value

The equivalent time in the item’s timebase.

## See Also

### Time Conversion

func itemTime(forHostTime: CFTimeInterval) -> CMTime

Converts a host time, specified in seconds, to the item’s timebase.

func itemTime(forMachAbsoluteTime: Int64) -> CMTime

Converts a Mach host time to the item’s timebase.


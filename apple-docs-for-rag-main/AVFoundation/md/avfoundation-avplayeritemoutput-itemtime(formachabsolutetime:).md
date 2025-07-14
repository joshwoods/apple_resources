

- AVFoundation
- AVPlayerItemOutput
-  itemTime(forMachAbsoluteTime:) 

Instance Method

# itemTime(forMachAbsoluteTime:)

Converts a Mach host time to the item’s timebase.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func itemTime(forMachAbsoluteTime machAbsoluteTime: Int64) -> CMTime
```

## Parameters 

`machAbsoluteTime`  

The Mach host time to convert. You typically retrieve this value using the `mach_absolute_time` function.

## Return Value

The equivalent time in the item’s timebase.

## See Also

### Time Conversion

func itemTime(forHostTime: CFTimeInterval) -> CMTime

Converts a host time, specified in seconds, to the item’s timebase.

func itemTime(for: CVTimeStamp) -> CMTime

Converts a Core Video timestamp to the item’s timebase.


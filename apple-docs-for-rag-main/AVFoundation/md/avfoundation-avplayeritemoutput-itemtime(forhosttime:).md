

- AVFoundation
- AVPlayerItemOutput
-  itemTime(forHostTime:) 

Instance Method

# itemTime(forHostTime:)

Converts a host time, specified in seconds, to the item’s timebase.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func itemTime(forHostTime hostTimeInSeconds: CFTimeInterval) -> CMTime
```

## Parameters 

`hostTimeInSeconds`  

A host time value, specified in seconds. For example, you might specify the time value returned by the CACurrentMediaTime() function or the timestamp from a CADisplayLink object for this parameter.

## Return Value

The equivalent time in the item’s timebase.

## Discussion

The timestamp associated with a CADisplayLink object represents the time of the most recent screen refresh, which is usually a time in the past. If you want to find the time associated with the next screen refresh, you need to increment the timestamp by the value in the display link’s `duration` property.

## See Also

### Time Conversion

func itemTime(forMachAbsoluteTime: Int64) -> CMTime

Converts a Mach host time to the item’s timebase.

func itemTime(for: CVTimeStamp) -> CMTime

Converts a Core Video timestamp to the item’s timebase.


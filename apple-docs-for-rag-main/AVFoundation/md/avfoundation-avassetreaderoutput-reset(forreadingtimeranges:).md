

- AVFoundation
- AVAssetReaderOutput
-  reset(forReadingTimeRanges:) 

Instance Method

# reset(forReadingTimeRanges:)

Restarts reading with a new set of time ranges.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func reset(forReadingTimeRanges timeRanges: [NSValue])
```

## Parameters 

`timeRanges`  

An array of NSValue objects, each representing a single CMTimeRange structure.

## Discussion

You may only call this method if the value of the supportsRandomAccess property is true. You can’t call it after invoking markConfigurationAsFinal().

A typical time to call this method is when performing multi-pass encoding using an instance of AVAssetWriter. In this case, call the copyNextSampleBuffer() method until it returns `nil`, and then ask the asset writer’s input for a set of time ranges to reencode. You pass the time ranges to this method to prepare the output for the next pass.

The time ranges that you set here override the value of the asset reader’s timeRange property. If the start times of the time range in the array don’t strictly increase, or if two or more time ranges in the array overlap, the system throws an exception. It’s an error to include a time range with a nonnumeric start time or duration, unless the duration is positiveInfinity.

If you call this method while the asset reader is in an AVAssetReader.Status.failed or AVAssetReader.Status.cancelled state, its status property value doesn’t change, and the result of the next call to copyNextSampleBuffer() is `nil`.

If you call this method while there’s still media data to read, the system throws an exception. You can only call it after the asset reader starts reading.

## See Also

### Configuring Reading

var alwaysCopiesSampleData: Bool

A Boolean value that indicates whether the output vends copied sample data.

var supportsRandomAccess: Bool

A Boolean value that indicates whether the output supports reconfiguring the time ranges it reads.

func markConfigurationAsFinal()

Tells the output that it’s finished reconfiguring time ranges, and allows the asset reader to advance to a completed state.


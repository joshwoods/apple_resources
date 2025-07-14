

- AVFoundation
- AVAssetReaderOutput
-  supportsRandomAccess 

Instance Property

# supportsRandomAccess

A Boolean value that indicates whether the output supports reconfiguring the time ranges it reads.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var supportsRandomAccess: Bool { get set }
```

## Discussion

The default value is false, which means you can’t reconfigure the output after reading begins. This setting may result in more efficient reading, particularly when you’re using multiple asset reader outputs.

A value of true indicates that you can reconfigure the output’s time ranges after reading begins by calling the reset(forReadingTimeRanges:) method. This setting also prevents the asset reader from progressing to a completed state until you call the markConfigurationAsFinal() method.

You can’t set this value after you call startReading() on the asset reader.

## See Also

### Configuring Reading

var alwaysCopiesSampleData: Bool

A Boolean value that indicates whether the output vends copied sample data.

func reset(forReadingTimeRanges: [NSValue])

Restarts reading with a new set of time ranges.

func markConfigurationAsFinal()

Tells the output that it’s finished reconfiguring time ranges, and allows the asset reader to advance to a completed state.


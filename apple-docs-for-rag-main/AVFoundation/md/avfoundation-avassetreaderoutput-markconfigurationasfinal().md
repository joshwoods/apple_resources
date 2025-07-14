

- AVFoundation
- AVAssetReaderOutput
-  markConfigurationAsFinal() 

Instance Method

# markConfigurationAsFinal()

Tells the output that it’s finished reconfiguring time ranges, and allows the asset reader to advance to a completed state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func markConfigurationAsFinal()
```

## Discussion

When the value of the supportsRandomAccess property is true, the asset reader doesn’t advance to an AVAssetReader.Status.completed state until you call this method.

After you call this method, you can’t make further calls to the reset(forReadingTimeRanges:) method.

When the destination of the output’s media data is an AVAssetWriterInput that you configure for multi-pass encoding, an appropriate time to call this method is after the asset writer input indicates that it doesn’t require performing additional passes.

## See Also

### Configuring Reading

var alwaysCopiesSampleData: Bool

A Boolean value that indicates whether the output vends copied sample data.

var supportsRandomAccess: Bool

A Boolean value that indicates whether the output supports reconfiguring the time ranges it reads.

func reset(forReadingTimeRanges: [NSValue])

Restarts reading with a new set of time ranges.


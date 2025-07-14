

- Model I/O
- MDLAsset
-  endTime 

Instance Property

# endTime

The timestamp for the last timed data sample in the asset.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var endTime: TimeInterval { get set }
```

## Discussion

Timed data in an asset is clamped to the start and end times—requesting sample data for a time sample after the start time returns the sample data at the end time.

If the asset does not contain timed information, this property’s value is zero.

## See Also

### Working with Timed Information

var frameInterval: TimeInterval

The time interval between data samples in the asset.

var startTime: TimeInterval

The timestamp for the first timed data sample in the asset.


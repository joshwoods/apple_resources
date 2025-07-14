

- Create ML Components
- TemporalSegmentIdentifier
-  range 

Instance Property

# range

The segment’s timestamp range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var range: Range
```

## Discussion

To get a timestamp in seconds divide the value by the timescale.

## See Also

### Getting the properties

var durationInSeconds: TimeInterval

The segment duration in seconds.

var rangeInSeconds: Range&lt;TimeInterval>

The time range in seconds.

var source: String

The segment source. For files use the full path or URL of the file.

var timescale: Int

The identifier’s timescale is the number of uniquely identifiable timestamps in a second.


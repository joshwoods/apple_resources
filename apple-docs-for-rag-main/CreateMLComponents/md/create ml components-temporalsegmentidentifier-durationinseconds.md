

- Create ML Components
- TemporalSegmentIdentifier
-  durationInSeconds 

Instance Property

# durationInSeconds

The segment duration in seconds.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var durationInSeconds: TimeInterval { get }
```

## See Also

### Getting the properties

var range: Range&lt;Int>

The segment’s timestamp range.

var rangeInSeconds: Range&lt;TimeInterval>

The time range in seconds.

var source: String

The segment source. For files use the full path or URL of the file.

var timescale: Int

The identifier’s timescale is the number of uniquely identifiable timestamps in a second.


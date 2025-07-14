

- Core Media
- CMTimeMapping
-  target 

Instance Property

# target

A time range on the target timeline.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
var target: CMTimeRange
```

## Discussion

If the target and source have different durations, the source segment should play at a rate of `source.duration / target.duration` to fit.

## See Also

### Accessing Time Ranges

var source: CMTimeRange

A time range on the source timeline.


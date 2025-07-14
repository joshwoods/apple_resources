

- AppKit
- NSTextLayoutManager
- NSTextLayoutManager.SegmentOptions
-  headSegmentExtended 

Type Property

# headSegmentExtended

Returns the value that causes the framework to extend the segment to the tail edge.

macOS 12.0+

``` source
static var headSegmentExtended: NSTextLayoutManager.SegmentOptions { get }
```

## See Also

### Getting segment options

static var middleFragmentsExcluded: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to enumerate segments in only the first and last line fragments.

static var rangeNotRequired: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework enumerate text segment rectangles, but avoids preparing a range object.

static var tailSegmentExtended: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to extend the segment to the tail edge.

static var upstreamAffinity: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to the place the segment based on the upstream affinity for an empty range.


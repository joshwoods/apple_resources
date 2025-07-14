

- UIKit
- NSTextLayoutManager
- NSTextLayoutManager.SegmentOptions
-  upstreamAffinity 

Type Property

# upstreamAffinity

Returns the value that causes the framework to the place the segment based on the upstream affinity for an empty range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
static var upstreamAffinity: NSTextLayoutManager.SegmentOptions { get }
```

## See Also

### Getting segment options

static var headSegmentExtended: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to extend the segment to the tail edge.

static var middleFragmentsExcluded: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to enumerate segments in only the first and last line fragments.

static var rangeNotRequired: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework enumerate text segment rectangles, but avoids preparing a range object.

static var tailSegmentExtended: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to extend the segment to the tail edge.


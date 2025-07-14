

- AppKit
- NSSegmentedControl
-  segmentDistribution 

Instance Property

# segmentDistribution

macOS 10.13+

``` source
@MainActor
var segmentDistribution: NSSegmentedControl.Distribution { get set }
```

## See Also

### Adjusting the Segment Spacing

func setWidth(CGFloat, forSegment: Int)

Sets the width of the specified segment.

func width(forSegment: Int) -> CGFloat

Returns the width of the specified segment.

enum Distribution

var activeCompressionOptions: NSUserInterfaceCompressionOptions

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize


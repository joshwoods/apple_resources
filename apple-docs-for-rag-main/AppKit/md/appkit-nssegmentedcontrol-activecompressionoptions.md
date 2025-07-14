

- AppKit
- NSSegmentedControl
-  activeCompressionOptions 

Instance Property

# activeCompressionOptions

macOS 10.13+

``` source
@NSCopying @MainActor
var activeCompressionOptions: NSUserInterfaceCompressionOptions { get }
```

## See Also

### Adjusting the Segment Spacing

func setWidth(CGFloat, forSegment: Int)

Sets the width of the specified segment.

func width(forSegment: Int) -> CGFloat

Returns the width of the specified segment.

var segmentDistribution: NSSegmentedControl.Distribution

enum Distribution

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize


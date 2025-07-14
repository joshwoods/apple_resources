

- AppKit
- NSSegmentedControl
-  minimumSize(withPrioritizedCompressionOptions:) 

Instance Method

# minimumSize(withPrioritizedCompressionOptions:)

macOS 10.13+

``` source
@MainActor
func minimumSize(withPrioritizedCompressionOptions prioritizedOptions: [NSUserInterfaceCompressionOptions]) -> NSSize
```

## See Also

### Adjusting the Segment Spacing

func setWidth(CGFloat, forSegment: Int)

Sets the width of the specified segment.

func width(forSegment: Int) -> CGFloat

Returns the width of the specified segment.

var segmentDistribution: NSSegmentedControl.Distribution

enum Distribution

var activeCompressionOptions: NSUserInterfaceCompressionOptions

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])


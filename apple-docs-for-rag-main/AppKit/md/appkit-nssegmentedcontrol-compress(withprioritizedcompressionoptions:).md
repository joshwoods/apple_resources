

- AppKit
- NSSegmentedControl
-  compress(withPrioritizedCompressionOptions:) 

Instance Method

# compress(withPrioritizedCompressionOptions:)

macOS 10.13+

``` source
@MainActor
func compress(withPrioritizedCompressionOptions prioritizedOptions: [NSUserInterfaceCompressionOptions])
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

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize


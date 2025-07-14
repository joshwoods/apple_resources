

- AppKit
- NSSegmentedControl
-  width(forSegment:) 

Instance Method

# width(forSegment:)

Returns the width of the specified segment.

macOS

``` source
@MainActor
func width(forSegment segment: Int) -> CGFloat
```

## Parameters 

`segment`  

The index of the segment whose width you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## Return Value

The width of the segment, measured in points, or 0 if the segment is sized to fit the available space automatically.

## See Also

### Adjusting the Segment Spacing

func setWidth(CGFloat, forSegment: Int)

Sets the width of the specified segment.

var segmentDistribution: NSSegmentedControl.Distribution

enum Distribution

var activeCompressionOptions: NSUserInterfaceCompressionOptions

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize




- AppKit
- NSSegmentedControl
-  setWidth(\_:forSegment:) 

Instance Method

# setWidth(\_:forSegment:)

Sets the width of the specified segment.

macOS

``` source
@MainActor
func setWidth(
    _ width: CGFloat,
    forSegment segment: Int
)
```

## Parameters 

`width`  

The width of the segment, measured in points. Specify the value `0` if you want the segment to be sized to fit the available space automatically.

`segment`  

The index of the segment whose width you want to set. This method raises an exception (rangeException) if the index is out of bounds.

## See Also

### Adjusting the Segment Spacing

func width(forSegment: Int) -> CGFloat

Returns the width of the specified segment.

var segmentDistribution: NSSegmentedControl.Distribution

enum Distribution

var activeCompressionOptions: NSUserInterfaceCompressionOptions

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize


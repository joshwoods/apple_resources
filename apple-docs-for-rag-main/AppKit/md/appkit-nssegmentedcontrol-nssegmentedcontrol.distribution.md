

- AppKit
- NSSegmentedControl
-  NSSegmentedControl.Distribution 

Enumeration

# NSSegmentedControl.Distribution

macOS 10.13+

``` source
enum Distribution
```

## Topics

### Distribution Options

case fit

case fill

case fillEqually

case fillProportionally

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Adjusting the Segment Spacing

func setWidth(CGFloat, forSegment: Int)

Sets the width of the specified segment.

func width(forSegment: Int) -> CGFloat

Returns the width of the specified segment.

var segmentDistribution: NSSegmentedControl.Distribution

var activeCompressionOptions: NSUserInterfaceCompressionOptions

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize


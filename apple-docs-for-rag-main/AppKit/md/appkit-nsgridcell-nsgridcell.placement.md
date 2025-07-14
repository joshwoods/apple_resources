

- AppKit
- NSGridCell
-  NSGridCell.Placement 

Enumeration

# NSGridCell.Placement

macOS 10.12+

``` source
enum Placement
```

## Topics

### Placement Options

static var top: NSGridCell.Placement

static var bottom: NSGridCell.Placement

case center

case fill

case inherited

case leading

case none

case trailing

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

### Formatting the Cell

var customPlacementConstraints: [NSLayoutConstraint]

var rowAlignment: NSGridRow.Alignment

var xPlacement: NSGridCell.Placement

var yPlacement: NSGridCell.Placement




- AppKit
-  NSGridColumn 

Class

# NSGridColumn

A column within a grid view.

macOS 10.12+

``` source
@MainActor
class NSGridColumn
```

## Topics

### Instance Properties

var gridView: NSGridView?

var isHidden: Bool

var leadingPadding: CGFloat

var numberOfCells: Int

var trailingPadding: CGFloat

var width: CGFloat

var xPlacement: NSGridCell.Placement

### Instance Methods

func cell(at: Int) -> NSGridCell

func mergeCells(in: NSRange)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Rows and Columns

class NSGridRow

A row within a grid view.


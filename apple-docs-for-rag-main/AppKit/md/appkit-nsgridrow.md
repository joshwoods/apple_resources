

- AppKit
-  NSGridRow 

Class

# NSGridRow

A row within a grid view.

macOS 10.12+

``` source
@MainActor
class NSGridRow
```

## Topics

### Getting the Row Details

var numberOfCells: Int

var isHidden: Bool

### Formatting the Row

var topPadding: CGFloat

var bottomPadding: CGFloat

var height: CGFloat

var rowAlignment: NSGridRow.Alignment

var yPlacement: NSGridCell.Placement

enum Alignment

### Getting the Grid View

var gridView: NSGridView?

### Getting Cells

func cell(at: Int) -> NSGridCell

### Merging Cells in the Row

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

class NSGridColumn

A column within a grid view.


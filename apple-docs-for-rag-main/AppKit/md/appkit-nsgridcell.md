

- AppKit
-  NSGridCell 

Class

# NSGridCell

An individual content area within a grid view, typically at the intersection of a row and a column.

macOS 10.12+

``` source
@MainActor
class NSGridCell
```

## Overview

Use a grid cell to specify the content view to display and to position the content view within the cell’s area.

## Topics

### Getting the Cell Containers

var column: NSGridColumn?

var row: NSGridRow?

var contentView: NSView?

class var emptyContentView: NSView

### Formatting the Cell

var customPlacementConstraints: [NSLayoutConstraint]

var rowAlignment: NSGridRow.Alignment

var xPlacement: NSGridCell.Placement

var yPlacement: NSGridCell.Placement

enum Placement

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


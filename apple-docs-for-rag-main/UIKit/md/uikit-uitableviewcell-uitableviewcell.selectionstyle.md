

- UIKit
- UITableViewCell
-  UITableViewCell.SelectionStyle 

Enumeration

# UITableViewCell.SelectionStyle

The style of selected cells.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum SelectionStyle
```

## Overview

You use these constants to set the value of the selectionStyle property.

## Topics

### Constants

case none

The cell has no distinct style for when it’s selected.

case blue

The cell has a default background color when it’s selected.

case gray

The cell has a gray background when it’s selected.

case `default`

The cell selection style to use for tables.

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

### Managing cell selection and highlighting

var selectionStyle: UITableViewCell.SelectionStyle

The style of selection for a cell.

var isSelected: Bool

A Boolean value that indicates whether the cell is selected.

func setSelected(Bool, animated: Bool)

Sets the selected state of the cell, optionally animating the transition between states.

var isHighlighted: Bool

A Boolean value that indicates whether the cell is highlighted.

func setHighlighted(Bool, animated: Bool)

Sets the highlighted state of the cell, optionally animating the transition between states.


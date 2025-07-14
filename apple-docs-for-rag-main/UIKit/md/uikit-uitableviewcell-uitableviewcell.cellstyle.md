

- UIKit
- UITableViewCell
-  UITableViewCell.CellStyle 

Enumeration

# UITableViewCell.CellStyle

An enumeration for the various styles of cells.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum CellStyle
```

## Overview

In all these cell styles, the larger of the text labels is accessed using the textLabel property and the smaller using the detailTextLabel property.

## Topics

### Cell styles

case `default`

A simple style for a cell with a text label (black and left-aligned) and an optional image view.

case value1

A style for a cell with a label on the left side of the cell with left-aligned and black text; on the right side is a label that has smaller blue text and is right-aligned.

case value2

A style for a cell with a label on the left side of the cell with text that’s right-aligned and blue; on the right side of the cell is another label with smaller text that’s left-aligned and black.

case subtitle

A style for a cell with a left-aligned label across the top and a left-aligned label below it in smaller gray text.

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

### Creating a table view cell

init(style: UITableViewCell.CellStyle, reuseIdentifier: String?)

Initializes a table cell with a style and a reuse identifier and returns it to the caller.

init?(coder: NSCoder)

Creates a table view from data in an unarchiver.


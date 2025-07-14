

- UIKit
- UITableViewCell
-  UITableViewCell.SeparatorStyle 

Enumeration

# UITableViewCell.SeparatorStyle

The style for cells to use as separators.

iOSiPadOSMac CatalystvisionOS

``` source
enum SeparatorStyle
```

## Overview

You use these constants to set the value of the separatorStyle property defined by UITableView.

## Topics

### Constants

case none

The separator cell has no distinct style.

case singleLine

The separator cell has a single line running across its width.

case singleLineEtched

The separator cell has double lines running across its width, giving it an etched look.

Deprecated

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

### Customizing the separator appearance

var separatorStyle: UITableViewCell.SeparatorStyle

The style for table cells to use as separators.

var separatorColor: UIColor?

The color of separator rows in the table view.

var separatorEffect: UIVisualEffect?

The effect to apply to table separators.

var separatorInset: UIEdgeInsets

The default inset of cell separators.

var separatorInsetReference: UITableView.SeparatorInsetReference

An indicator of how to interpret the separator inset value.

enum SeparatorInsetReference

Constants that indicate how to interpret the separator inset value of a table view.


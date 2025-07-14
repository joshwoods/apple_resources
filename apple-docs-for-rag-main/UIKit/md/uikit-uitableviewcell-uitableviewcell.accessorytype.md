

- UIKit
- UITableViewCell
-  UITableViewCell.AccessoryType 

Enumeration

# UITableViewCell.AccessoryType

The type of standard accessory control used by a cell.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum AccessoryType
```

## Mentioned in 

Configuring the cells for your table

## Overview

Use these constants to set the value of the accessoryType property.

Several accessory views support additional interactions. For example, a detail button conveys that there is additional information for the user to see. For information about how to respond to interactions with a specific accessory view, see the discussion for that type.

## Topics

### Accessory views

case none

No accessory view.

case disclosureIndicator

A chevron-shaped control for presenting new content.

case detailDisclosureButton

An information button and a disclosure (chevron) control.

case checkmark

A checkmark image.

case detailButton

An information button.

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

### Managing accessory views

var accessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s normal state.

var accessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s normal state.

var editingAccessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s editing state.

var editingAccessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s editing state.


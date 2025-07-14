

- UIKit
- UITableViewCell
- UITableViewCell.AccessoryType
-  UITableViewCell.AccessoryType.checkmark 

Case

# UITableViewCell.AccessoryType.checkmark

A checkmark image.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case checkmark
```

## Mentioned in 

Handling row selection in a table view

## Discussion

Choose this option to display a checkmark image. This type of accessory view doesn’t track touches.

To hide or show a check mark for a row, toggle the accessoryType property of the cell between the UITableViewCell.AccessoryType.none and UITableViewCell.AccessoryType.checkmark values. For example, if you use a checkmark to indicate one selected row from a group of rows, use your delegate’s tableView(_:didSelectRowAt:) method to update the accessory views of the affected rows.

## See Also

### Accessory views

case none

No accessory view.

case disclosureIndicator

A chevron-shaped control for presenting new content.

case detailDisclosureButton

An information button and a disclosure (chevron) control.

case detailButton

An information button.


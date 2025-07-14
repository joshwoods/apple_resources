

- UIKit
- UITableViewCell
- UITableViewCell.AccessoryType
-  UITableViewCell.AccessoryType.detailButton 

Case

# UITableViewCell.AccessoryType.detailButton

An information button.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case detailButton
```

## Discussion

Choose this option to display a button that, when tapped, displays information about the row. Use your delegate’s tableView(_:accessoryButtonTappedForRowWith:) method to respond to taps in the button.

## See Also

### Accessory views

case none

No accessory view.

case disclosureIndicator

A chevron-shaped control for presenting new content.

case detailDisclosureButton

An information button and a disclosure (chevron) control.

case checkmark

A checkmark image.




- UIKit
- UITableViewCell
- UITableViewCell.AccessoryType
-  UITableViewCell.AccessoryType.detailDisclosureButton 

Case

# UITableViewCell.AccessoryType.detailDisclosureButton

An information button and a disclosure (chevron) control.

iOSiPadOSMac CatalystvisionOS

``` source
case detailDisclosureButton
```

## Discussion

Choose this type when you want both an information button and a disclosure control. Connect the disclosure control to a push segue to display new content. Use the delegate’s tableView(_:accessoryButtonTappedForRowWith:)method to respond to touch events in the detail button.

## See Also

### Accessory views

case none

No accessory view.

case disclosureIndicator

A chevron-shaped control for presenting new content.

case checkmark

A checkmark image.

case detailButton

An information button.


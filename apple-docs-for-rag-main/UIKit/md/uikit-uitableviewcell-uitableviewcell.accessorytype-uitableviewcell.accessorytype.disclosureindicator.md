

- UIKit
- UITableViewCell
- UITableViewCell.AccessoryType
-  UITableViewCell.AccessoryType.disclosureIndicator 

Case

# UITableViewCell.AccessoryType.disclosureIndicator

A chevron-shaped control for presenting new content.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case disclosureIndicator
```

## Discussion

Choose this type when you want taps in the accessory view to display new content. Connect the accessory view itself to a push segue to display that content.

The table view doesn’t call the delegate’s tableView(_:accessoryButtonTappedForRowWith:) method in response to touch events in this accessory view.

## See Also

### Accessory views

case none

No accessory view.

case detailDisclosureButton

An information button and a disclosure (chevron) control.

case checkmark

A checkmark image.

case detailButton

An information button.


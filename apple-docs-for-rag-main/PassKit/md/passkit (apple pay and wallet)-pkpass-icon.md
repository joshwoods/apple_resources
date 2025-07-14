

- PassKit (Apple Pay and Wallet)
- PKPass
-  icon 

Instance Property

# icon

The pass icon.

iOSiPadOSMac CatalystvisionOS

``` source
@NSCopying
var icon: UIImage { get }
```

## Discussion

You can use this property to display a pass’s icon as part of a UI element that represents the pass, such as a cell in a table view.

## See Also

### Getting the display attributes

func localizedValue(forFieldKey: String) -> Any?

Returns the localized value for a specified field of the pass.

var organizationName: String

The name of the organization that creates the pass.

var relevantDate: Date?

The date when the pass is most likely to be useful or necessary.

Deprecated


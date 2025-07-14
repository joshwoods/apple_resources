

- PassKit (Apple Pay and Wallet)
- PKPass
-  organizationName 

Instance Property

# organizationName

The name of the organization that creates the pass.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var organizationName: String { get }
```

## Discussion

You can use this property to display information about the organization that creates the pass as part of a user interface element that represents the pass, such as a cell in a table view.

## See Also

### Getting the display attributes

var icon: UIImage

The pass icon.

func localizedValue(forFieldKey: String) -> Any?

Returns the localized value for a specified field of the pass.

var relevantDate: Date?

The date when the pass is most likely to be useful or necessary.

Deprecated


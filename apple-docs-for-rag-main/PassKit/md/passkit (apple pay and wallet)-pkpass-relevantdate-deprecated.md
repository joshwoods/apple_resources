

- PassKit (Apple Pay and Wallet)
- PKPass
-  relevantDate Deprecated

Instance Property

# relevantDate

The date when the pass is most likely to be useful or necessary.

iOS 6.0–18.0DeprecatediPadOS 6.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 2.0–11.0Deprecated

``` source
var relevantDate: Date? { get }
```

Deprecated

Use relevantDates

## Discussion

You can use this property for sorting UI elements that represent passes, such as cells in a table view.

## See Also

### Getting the display attributes

var icon: UIImage

The pass icon.

func localizedValue(forFieldKey: String) -> Any?

Returns the localized value for a specified field of the pass.

var organizationName: String

The name of the organization that creates the pass.


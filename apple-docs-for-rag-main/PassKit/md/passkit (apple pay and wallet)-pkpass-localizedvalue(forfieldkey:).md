

- PassKit (Apple Pay and Wallet)
- PKPass
-  localizedValue(forFieldKey:) 

Instance Method

# localizedValue(forFieldKey:)

Returns the localized value for a specified field of the pass.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
func localizedValue(forFieldKey key: String) -> Any?
```

## Parameters 

`key`  

The field’s key as specified in the pass.

## Return Value

The localized value for the pass’s field.

## Discussion

If your app works with passes from arbitrary sources, such as an email client, it can’t use this method because PassKit doesn’t know the keys for those passes in advance. Use the other properties of this class, such as organizationName, instead.

## See Also

### Getting the display attributes

var icon: UIImage

The pass icon.

var organizationName: String

The name of the organization that creates the pass.

var relevantDate: Date?

The date when the pass is most likely to be useful or necessary.

Deprecated


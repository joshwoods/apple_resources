

- Contacts
- CNPostalAddress
-  localizedString(forKey:) 

Type Method

# localizedString(forKey:)

Returns the localized name for the property associated with the specified key.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func localizedString(forKey key: String) -> String
```

## Parameters 

`key`  

The key for the property whose localized name is being returned.

## Return Value

The localized property name.

## See Also

### Getting Localized Postal Values

let CNPostalAddressStreetKey: String

The street name of the address.

let CNPostalAddressCityKey: String

The city of the address.

let CNPostalAddressStateKey: String

The state name of the address.

let CNPostalAddressPostalCodeKey: String

The postal code of the address.

let CNPostalAddressCountryKey: String

The country or region name of the address.

let CNPostalAddressISOCountryCodeKey: String

The ISO country code of the address.


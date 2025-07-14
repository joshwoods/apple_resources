

- Core Location
- CLPlacemark
-  addressDictionary Deprecated

Instance Property

# addressDictionary

A dictionary containing the Address Book keys and values for the placemark.

iOS 5.0–11.0DeprecatediPadOS 5.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.13DeprecatedtvOS 9.0–11.0DeprecatedwatchOS 1.0–4.0Deprecated

``` source
var addressDictionary: [AnyHashable : Any]? { get }
```

Deprecated

Use CLPlacemark instead of Address Book.

## Discussion

The keys in this dictionary are those defined by the Address Book framework and used to access address information for a person. For a list of the strings that can be in this dictionary, see the “Address Property” constants in `ABPerson`.

You can format the contents of this dictionary to get a full address string as opposed to building the address yourself. To format the dictionary, use the ABCreateStringWithAddressDictionary(_:_:) function as described in `AddressBookUI Functions`.

## See Also

### Getting the associated contact details

var postalAddress: CNPostalAddress?

The postal address associated with the location, formatted for use with the Contacts framework.

